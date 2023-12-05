<script setup>
definePageMeta({
  layout: "docs",
});

const consoleLog = `console.log('hello')`;
const code = `<TextesCode code="${consoleLog}" language="js" />`;
</script>

<template>
  <Container>
    <TitresH1>Textes</TitresH1>

    <TextesParagraphe>
      Utilisez les composants de texte pour afficher des paragraphes ou des
      blocks de code, etc.
    </TextesParagraphe>

    <TitresH2>Paragraphe</TitresH2>

    <TextesParagraphe>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam
      voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas
      voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates
      quia quae voluptatem, quos quod quas voluptatibus quidem doloribus.
    </TextesParagraphe>
    <TextesCode :code="`<TextesParagraphe>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus.
</TextesParagraphe>`" />

    <TitresH2>Code</TitresH2>

    <TextesParagraphe> Language par défaut : vue </TextesParagraphe>

    <TextesCode :code="consoleLog" language="js" />

    <TextesCode :code="code" />

    <TitresH2>Gras</TitresH2>

    <TextesParagraphe>
      <TextesGras> Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates
        quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates
        quia
        quae voluptatem, quos quod quas voluptatibus quidem doloribus. </TextesGras>
    </TextesParagraphe>

    <TextesCode :code="`<TextesParagraphe><TextesGras>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus.
</TextesGras></TextesParagraphe>`" />

    <TitresH2>Italique</TitresH2>

    <TextesParagraphe>
      <TextesItalique> Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates
        quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates
        quia
        quae voluptatem, quos quod quas voluptatibus quidem doloribus. </TextesItalique>
    </TextesParagraphe>

    <TextesCode :code="`<TextesParagraphe><TextesItalique>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus.
</TextesItalique</TextesParagraphe>`" />

    <TitresH2>Souligne</TitresH2>

    <TextesParagraphe>
      <TextesSouligne> Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates
        quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates
        quia
        quae voluptatem, quos quod quas voluptatibus quidem doloribus. </TextesSouligne>
    </TextesParagraphe>

    <TextesCode :code="`<TextesParagraphe><TextesSouligne>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus.
</TextesSouligne></TextesParagraphe>`" />
  </Container>
</template>
