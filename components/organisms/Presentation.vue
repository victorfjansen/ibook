<template>
  <main class="presentation">
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste alias sint,
    distinctio sunt iure laboriosam quaerat dolorum! Distinctio numquam sunt
    iste eligendi unde porro ducimus laborum reprehenderit recusandae repellat.
    Tempore?
    <img src="@/assets/img/presentation.svg" alt="Apresentação do Ibook" />
  </main>
</template>

<style scoped lang="scss">
.presentation {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 2rem;
  align-items: center;
  @include screen('small', 'medium') {
    grid-template-columns: 1fr;
  }
  p {
    line-height: 26px;
  }
  img {
    max-width: 100%;
  }
}
</style>
