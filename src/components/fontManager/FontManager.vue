<template>
    <div id="fontmanagercontent" style="display:none; width:720px;">
        <div class="font-picker" style="margin-bottom: 10px;">
            <h1 class="tab_title" i18n="osdSetupFontPresets"></h1>
            <!-- Font preview and list -->
            <label class="font-manager-version-info"></label>
            <div class="content_wrapper font-preview"></div>
            <div class="fontpresets_wrapper">
                <label id="font-selector-label" i18n="osdSetupFontPresetsSelector"></label>
                <select class="fontpresets">
                    <option value="-1" disabled i18n="osdSetupFontPresetsSelectorCustomOption"></option>
                    <!-- Other values populated at runtime -->
                </select>
                <span id="font-selector-span" i18n="osdSetupFontPresetsSelectorOr"> Or </span>
            </div>

            <!-- Boot logo setup -->
            <LogoManager />
            
            <!-- Upload progress bar -->
            <div class="info">
                <a name="progressbar"></a>
                <progress class="progress" value="0" min="0" max="100"></progress>
                <div class="progressLabel" style="margin-top: -21px; width: 95%; text-align: center; position: absolute;"></div>
            </div>
        </div>
        <!-- Upload button -->
        <div class="default_btn green" style="width:100%; float:left;
            ">
            <a class="flash_font active" i18n="osdSetupUploadFont"></a>
        </div>
    </div>    
</template>

<script lang="ts">
import Vue from 'vue'
import LogoManager from 'logoManager/LogoManager.vue'
export default Vue.extend({
    components: {
        'LogoManager': LogoManager,
    },
})
</script>