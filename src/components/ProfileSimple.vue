<template>
    <div class="profile-simple d-flex">
        <b-avatar :src="avatar" :alt="name" />
        <div class="info small">
            <p class="name">{{name}}</p>
            <p class="text-muted">@{{username}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ProfileSimple',
    props: {
        name: '',
        username: '',
        avatar: ''
    }
}
</script>

<style scoped>
.profile-simple p { margin: 0; margin-left: 15px; padding: 0 }
.profile-simple p.name { font-weight: 600; }
</style>