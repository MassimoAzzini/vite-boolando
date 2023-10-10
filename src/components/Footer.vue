<script>
export default {
  name: 'Footer',
  
}
</script>

<template>

  <footer>

    <div class="container flex">
      <div class="company">
        <span>Booleando s.r.l.</span>
        <nav>
          <ul class="flex">
            <li><a href="#" target="_self">Informazioni legali</a></li>
            <li><a href="#" target="_self">Informativa sulla privacy</a></li>
            <li><a href="#" target="_self">Diritto di recesso</a></li>
          </ul>
        </nav>
      </div>

      <div class="social">
        <span>Trovaci anche su</span>
        <nav>
          <ul class="flex">
            <li><a href="#" target="_blank"><i class="fa-brands fa-square-twitter"></i></a></li>
            <li><a href="#" target="_blank"><i class="fa-brands fa-square-facebook"></i></a></li>
            <li><a href="#" target="_blank"><i class="fa-brands fa-square-instagram"></i></a></li>
            <li><a href="#" target="_blank"><i class="fa-brands fa-square-pinterest"></i></a></li>
            <li><a href="#" target="_blank"><i class="fa-brands fa-square-youtube"></i></a></li>
          </ul>
        </nav>

      </div>
    </div>

  </footer>
  
</template>

<style lang="scss" scoped>

footer {
  background-color: black;
  height: 100px;
}

footer .container.flex {
  height: 100%;
  justify-content: space-between;
  align-items: center;
}

footer .company span {
  font-weight: bold;
  font-size: 1rem;
}

footer .company span,
footer .social span {
  margin: 0 5px;
}

footer .company > *,
footer .social > * {
  margin-top: 10px;
  margin-bottom: 10px;
}

footer .social a {
  font-size: 1rem;
}

</style>