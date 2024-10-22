<template>
  <div>
    <AppHeader />
    <AppLoader />
    <AppFooter />
  </div>
</template>

<style scoped>
  @font-face {
      font-family: OpenSans;
      src: url('../fonts/OpenSans-VariableFont_wdth\,wght.ttf')
  }

  * {
      font-family: OpenSans, sans-serif;
      list-style: none;
  }

  *::-webkit-scrollbar {
      display: none;
    }

  body {
      overflow-x:hidden;
  }

  h2 {
      margin-left:1.5rem;
  }

  footer {
      margin-top: 2rem;
  }
  footer nav {
      padding:1rem;
  }
  footer nav h2 {
      margin:calc(-1rem - 1px) calc(-1rem - 1px) 1rem 2rem
  }

  ::marker {
      color: currentColor;
  }

  section a {
      padding:0 .25rem
  }
  a:focus {
      outline:none;
      background: var(--attention);  
      color: var(--white);
  }
</style>