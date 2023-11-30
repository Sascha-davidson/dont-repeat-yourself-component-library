<script>
  import Input from "$lib/atoms/input.svelte";
  import InputRequired from "$lib/atoms/input-required.svelte";
  import Taxtarea from "$lib/atoms/textarea.svelte";

  export let FormID, Method, Action
</script>

<form id="{FormID}" method="{Method}" action="{Action}">
  <InputRequired
    InputType="text"
    InputID="AddPlayer"
    LableFor="AddPlayer"
    LableText="* Add player ..."
  />
  <section>
    <Input
      InputType="Date"
      InputID="BirthDate"
      LableFor="BirthDate"
      LableText="Date of birth..."
    />
    <InputRequired
      InputType="text"
      InputID="JerseyNumber"
      LableFor="JerseyNumber"
      LableText="* Jersey number..."
    />
  </section>
  <Input
    InputType="text"
    InputID="BirthCountry"
    LableFor="BirthCountry"
    LableText="* Country of birth..."
  />
  <Input
    InputType="text"
    InputID="ResidencePlace"
    LableFor="ResidencePlace"
    LableText="Place of residence..."
  />

  <Taxtarea InputID="Bio" LableFor="Bio" LableText="Bio..." />
</form>

<style>
  form {
    grid-area: form;
  }

  form {
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
    padding: 0.5rem 2rem 0.5rem 5px;
    overflow: auto;
    padding-top: 1.5rem;
  }

  form::-webkit-scrollbar-track {
    border-radius: 10px;
  }

  form::-webkit-scrollbar {
    width: 12px;
  }

  form::-webkit-scrollbar-thumb {
    border-radius: 10px;
    /* -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3); */
    background-color: #a7a7a7;
  }

  section {
    display: flex;
    gap: 2rem;
  }
</style>
