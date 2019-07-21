<template>
    <div class="sidebar" >
        <div class="sidebar-item active">
            <img class="sidebar-item-icon" src="@/assets/dashboard.svg">
            <span class="sidebar-item-title">Dashboard</span>
        </div>

        <div class="sidebar-item">
            <img class="sidebar-item-icon" src="@/assets/currently-live.svg">
            <span class="sidebar-item-title">Currently Live</span>
        </div>

        <div class="sidebar-item">
            <img class="sidebar-item-icon" src="@/assets/courses.svg">
            <span class="sidebar-item-title">Courses</span>
        </div>
        <div class="sidebar-item">
            <img class="sidebar-item-icon" src="@/assets/playlist.svg">
            <span class="sidebar-item-title">Playlist</span>
        </div>
        <div class="sidebar-item">
            <img class="sidebar-item-icon" src="@/assets/forum.svg">
            <span class="sidebar-item-title">Forum</span>
        </div>
    </div>
</template>

<script>
export default {
    name: "Sidebar",
    data () {
        return {
        }
    },
    methods: {
    }
}
</script>

<style scope>
.sidebar {
    padding-top: 10px;
    position: fixed;
    left: 0;
    align-items: center;
    width: 12em;
    height: 100vh;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    z-index: 999;
    -webkit-transition: 0.3s width;
    transition: 0.3s width;
    background-color: #F4F6FA;
    border-right: 1px solid #EEF0F2;
}

.sidebar-item {
    height:115px;
    width:140px;
    border-radius: 12px;
    flex-direction: column;
    display:flex;
    justify-content:space-around;
    align-items:center;
}

.sidebar-item-icon {
    height:38px;
    width:38px;
    margin-top:10px;
}

.sidebar-item-title {
    margin-bottom:10px;
    font-size: 16px;
    color: #707070;
}

.sidebar-item.active {
    background-color:#FF7448;

}

.sidebar-item.active>.sidebar-item-title {
    color:white;

}
</style>
