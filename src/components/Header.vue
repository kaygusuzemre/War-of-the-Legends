<template>
    <div class="headerr px-5 m-0" style="width:100%">
        <div class="position-absolute"></div>
        <b-navbar toggleable="lg" type="dark" class="navbar px-5">
            <b-navbar-brand href="#">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/LoL_icon.svg/1200px-LoL_icon.svg.png"
                    alt="" class="" height="60px" width="60px">
            </b-navbar-brand>
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
            <b-collapse id="nav-collapse" is-nav class="row-cols-2 justify-content-between align-items-center">
                <b-navbar-nav>
                    <b-nav-item href="#">Heroes</b-nav-item>
                    <b-nav-item href="#">Strategies</b-nav-item>
                </b-navbar-nav>

                <!-- Right aligned nav items -->
                <b-navbar-nav class="justify-content-end align-items-center">
                    <b-nav-form class="px-3">
                        <b-form-input size="m" class="mr-sm-2 bg-dark text-light" placeholder="Heroes">
                        </b-form-input>
                    </b-nav-form>
                    <b-button size="m" class="me-2 my-sm-0" type="submit">Search</b-button>

                    <b-nav-item-dropdown text="Lang">
                        <b-dropdown-item href="#">EN</b-dropdown-item>
                        <b-dropdown-item href="#">ES</b-dropdown-item>
                        <b-dropdown-item href="#">RU</b-dropdown-item>
                        <b-dropdown-item href="#">FA</b-dropdown-item>
                        <b-dropdown-item href="#">TR</b-dropdown-item>
                    </b-nav-item-dropdown>

                    <b-nav-item-dropdown>
                        <template #button-content>
                            <em>User</em>
                        </template>
                        <b-dropdown-item href="#">Profile</b-dropdown-item>
                        <b-dropdown-item href="#">Sign Out</b-dropdown-item>
                    </b-nav-item-dropdown>
                </b-navbar-nav>
            </b-collapse>
        </b-navbar>
    </div>
</template>

<script>
export default {
    name: "HeaderFirst",
};
</script>

<style>
.headerr {
    position: fixed;
    /* display: flex;
    justify-content: space-between; */
    z-index: 2;
    right: 50%;
    transform: translateX(50%);
    backdrop-filter: blur(4px);
}
</style>
