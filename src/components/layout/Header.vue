<template>
    <div class="header">
        <b-row>
            <b-col cols="2">
                <div class="header-logo">
                    <img src="@/assets/logo_iac.png">
                </div>
            </b-col>
            <b-col class="notification" cols="1" offset="7">
                <img class="notification-icon" src="@/assets/bell-icon.svg">
            </b-col>
            <b-col class="header-profile-section" cols="2">
                <img class="header-avatar" src="@/assets/avatar2.png">
                <div class="header-user">
                    <p class="header-user-username">Bob Marley</p>
                    <p class="header-user-role">member</p>
                </div>
                <img class="header-profile-dropdown-button" src="@/assets/down-arrow.svg">
            </b-col> 
        </b-row>
    </div>
</template>

<script>
// import store from '../../store'
export default {
    name: "Header",
}
</script>

<style scope>
.header {
    z-index: 1000;
    border-bottom: 1px solid #EEF0F2;
}
.header-logo {
    border-right: 1px solid #EEF0F2;
    background-color: #F4F6FA;
    padding: 7px;
    height: 60px;
    width:12em;
    display:flex;
    justify-content:center;
    align-items:center;
}

.notification {
    display:flex;
    align-items:center;
    justify-content:center;
    border-right:1px solid #EEF0F2;
}

.header-profile-section {
    display:flex;
    align-items:center;
}

.header-avatar {
    height:40px;
    width:40px;
    border-radius:50px;
}

.header-user {
    text-align:left;
    margin-left:20px;
}

.header-user-username {
    font-size:12px;
    margin:0;
    font-weight:600;
}

.header-user-role {
    font-size:12px;
    margin:0;
}

.notification-icon {
    height:23px;
    width:15px;
    cursor: pointer;
}

.header-profile-dropdown-button {
    height:20px;
    width:20px;
    border-radius:50px;
    background-color:yellow;
    margin-left:30px;
    cursor: pointer;
}
</style>
