<template>
  <TopNavigation/>
  <div class="p-2">
    {{ userStore.firstName }}
  </div>
</template>

<script setup>
// import PostsSection from '../../components/partials/profile/PostsSection.vue'
// import RouterLinkButton from '../../components/global/RouterLinkButton.vue'
// import ProfileInfoSection from '../../components/partials/profile/ProfileInfoSection.vue'
// import ProfileAboutSection from '../../components/partials/profile/ProfileAboutSection.vue'
// import SongsSection from '../../components/partials/profile/SongsSection.vue'
// import YoutubeVideosSection from '../../components/partials/profile/YoutubeVideosSection.vue'
import {useUserStore} from '../../store/user-store'
// import {useProfileStore} from '../../store/profile-store'
import {onMounted} from 'vue'
import TopNavigation from "@/components/structure/TopNavigation";
// import {useRoute} from 'vue-router'

// const route = useRoute()
const userStore = useUserStore()
// const profileStore = useProfileStore()
onMounted(async () => {
  // await profileStore.fetchProfileById(route.params.id)
})
</script>