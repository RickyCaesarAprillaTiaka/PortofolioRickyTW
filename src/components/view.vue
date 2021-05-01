<template>
<InstaFeed token="IGQVJVQndtdng4S3o0SEMxOUpONTFJenpfVHo3bVV0U2tIaUl1NDFoSlZATblFfa2h4dzcwSzJjSWc4SWhRTmRuYXFhME52MHlXd0dQc1NEZAVhFTDVIWUdpTEpaR3FQbm4tek94RGNhMmk2LTJrQTJkcgZDZD" fields="media_url,media_type,caption,permalink" container-class="image-container" :mediatypes="['IMAGE']" />
</template>

<script>
import InstaFeed from './InstaFeed'
    export default {
        name: 'Profile',
        components: {
            InstaFeed
        },
        props: {
            msg: String,
            msg2: String,
        },
        variants: {
            extend: {
                boxSizing: false,
            }
        },
    }
</script>