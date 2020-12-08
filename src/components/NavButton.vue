<template>
    <div class="nav-button">
        <p>{{ name }}</p>
    </div>
</template>

<script>
export default {
    name: 'NavButton',
    props: {
        name: name
    }
}
</script>

<style scoped>
.nav-button {
    width: 80%;
    margin: 0px 0px 5px 0px;
    cursor: pointer;
    border-radius: 4px;
    background-color: #2d3d56;
    border: none;
    color: #FFFFFF;
    text-align: center;
    font-size: 20px;
    padding: 18px;
    transition: all 0.5s;
    font-family: Palatino, Palatino Linotype, Palatino LT STD, Book Antiqua, Georgia, serif;
}

.nav-button span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.nav-button span:after {
  content: '\00bb';
  position: absolute;
  opacity: 0;
  top: 0;
  right: -10px;
  transition: 0.5s;
}

.nav-button:hover span {
  padding-right: 5px;
}

.nav-button:hover span:after {
  opacity: 1;
  right: 0;
}

</style>