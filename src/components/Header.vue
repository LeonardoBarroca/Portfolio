<template>
    <div class="navbar">
        <ul class="navbar-menu">
            <li><a href="#">Projeto 1</a></li>
            <li><a href="#">Projeto 2</a></li>
            <li><a href="#">Projeto 3</a></li>
        </ul>
    </div>
</template>
  
<script>
export default {
    name: "Header"

};
</script>
  
<style scoped>
.navbar {
    background-color: #063940;
    color: #fff;
    display: flex;
    align-items: center;
    padding: 16px;
}

.navbar-menu {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
}

.navbar-menu li {
    margin-right: 16px;

}

.navbar-menu li a {
    text-decoration: none;
    color: #fff;
}

@media (max-width: 768px) {
    .navbar {
        flex-direction: column;
    }

    .navbar-menu {
        display: flex;
        flex-direction: column;
    }

    .navbar-menu li {
        margin-right: 0;
    }

    .navbar-menu>*:not(:last-child) {
        margin-bottom: 16px;
    }
}
</style>
  