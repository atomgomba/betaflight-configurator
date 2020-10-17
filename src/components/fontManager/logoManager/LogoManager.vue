<template>
    <!-- Boot logo setup -->
    <div>
    <h1 class="tab_title" i18n="osdSetupCustomLogoTitle"></h1>
    <div class="grid-row">
        <div id="font-logo-preview-container" class="content_wrapper grid-col col6">
            <div id="font-logo-preview">
                <!-- this will be resized at runtime -->
            </div>
        </div>
        <div id="font-logo-info grid-col col6">
            <h3 i18n="osdSetupCustomLogoInfoTitle"></h3>
            <ul>
                <li id="font-logo-info-size" i18n="osdSetupCustomLogoInfoImageSize"></li>
                <li id="font-logo-info-colors" i18n="osdSetupCustomLogoInfoColorMap"></li>
            </ul>
            <p id="font-logo-info-upload-hint" i18n="osdSetupCustomLogoInfoUploadHint"></p>
        </div>
    </div>
    <!-- Replace logo button -->
    <div class="default_btn" style="width:100%; float:left;">
        <a class="replace_logo" i18n="osdSetupCustomLogoOpenImageButton"></a>
    </div>
    </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    props: {
        font: null,
    },
})
</script>