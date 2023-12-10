<script setup>
definePageMeta({
  layout: "docs",
});

const consoleLog = `console.log('hello')`;
const code = `<TextesCode code="${consoleLog}" language="js" />`;
</script>

<template>
  <Container>
    <TitresH1>Formulaires</TitresH1>

    <TextesParagraphe>
      Développez des composants pour les champs de formulaire : input number, email, checkbox, select, radio.
      Testez la fonctionnalité et l'accessibilité de chaque composant.
    </TextesParagraphe>

    <TitresH2>Input number</TitresH2>

    <TextesParagraphe>
      <FormsInputNumber>

      </FormsInputNumber>
    </TextesParagraphe>
    <TextesCode :code="`<FormsInputNumber>

      </FormsInputNumber>`" />

    <TitresH2>Code</TitresH2>

    <TextesParagraphe> Language par défaut : vue </TextesParagraphe>

    <TextesCode :code="consoleLog" language="js" />

    <TextesCode :code="code" />


  </Container>
</template>
