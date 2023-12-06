<script setup>
definePageMeta({
  layout: "docs",
});

const consoleLog = `console.log('hello')`;
const code = `<TextesCode code="${consoleLog}" language="js" />`;
</script>

<template>
  <Container>
    <TitresH1>User card</TitresH1>

    <TextesParagraphe>
      Utilisez les composants de texte pour afficher des paragraphes ou des
      blocks de code, etc.
    </TextesParagraphe>

    <CardsUser>
      TODO
      <template v-slot:avatar>
        <!-- content for the avatar slot -->
        <img src="../../../public/img/test.png" alt="">
      </template>
      <template #fullname>
        <!-- content for the info slot -->
        John Doe
      </template>
      <template #info>
        <!-- content for the info slot -->
        web developper since 2015
      </template>
    </CardsUser>

    <TextesCode :code="`<TextesParagraphe>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus. Quisquam voluptatum, quibusdam, voluptates quia quae voluptatem, quos quod quas voluptatibus quidem doloribus.
</TextesParagraphe>`" />

  </Container>
</template>
