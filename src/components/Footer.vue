<template>
    <div class="py-4 text-light">
        <b-navbar class="py-4 justify-content-center text-center">
            <b-navbar-nav class="text-capitalize">
                <b-nav-item>home</b-nav-item>
                <b-nav-item>features</b-nav-item>
                <b-nav-item>FAQs</b-nav-item>
                <b-nav-item>about</b-nav-item>
            </b-navbar-nav>
        </b-navbar>
        <div class="d-flex justify-content-center">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/LoL_icon.svg/1200px-LoL_icon.svg.png"
                alt="logo" style="width:130px" height="130px">
        </div>
        <div class="text-center py-4">
            <p>© Developed by <a href="https://github.com/kaygusuzemre" class="text-decoration-none"><span
                        class="span-footer">Emre
                        Kaygusuz</span></a></p>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterOne",
};
</script>

<style>
.span-footer,
a {
    color: black;
}
</style>