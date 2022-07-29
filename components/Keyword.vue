<template>
  <div>
    <b-form-tags v-model="value" no-outer-focus class="mb-2 download-tag">
      <template v-slot="{ tags, inputAttrs, inputHandlers, removeTag }">
        <div class="d-inline-block add-tag-style">
          <ul
            id="my-custom-tags-list"
            class="list-unstyled d-inline-flex flex-wrap mb-0"
            aria-live="polite"
            aria-atomic="false"
            aria-relevant="additions removals"
          >
            <!-- Always use the tag value as the :key, not the index! -->
            <!-- Otherwise screen readers will not read the tag
               additions and removals correctly -->
            <b-card
              v-for="tag in tags"
              :key="tag"
              :id="`my-custom-tags-tag_${tag.replace(/\s/g, '_')}_`"
              tag="li"
              class="mt-1 mr-1"
              body-class="py-1 pr-2 text-nowrap"
            >
              <strong>{{ tag }}</strong>
              <b-button
                @click="removeTag(tag)"
                variant="link"
                size="sm"
                :aria-controls="`my-custom-tags-tag_${tag.replace(
                  /\s/g,
                  '_'
                )}_`"
                ><b-img src="~assets/i/cross.svg" alt=""
              /></b-button>
            </b-card>
          </ul>

          <input
            v-bind="inputAttrs"
            v-on="inputHandlers"
            placeholder="Enter Keywords..."
            class="form-control"
          />
        </div>
        
      </template>
    </b-form-tags>
  </div>
</template>

<script>
export default {
  data() {
    return {
      value: ["Published", "Last Week", "English"],
    };
  },
};
</script>

<style scoped>

.download-tag {
  position: relative;
  
}
.download-tag a  {
       position: absolute;
    top: 50%;
    right: 0;
    transform: translate(-19px, -50%);
    border: 0;
}
ul#my-custom-tags-list li[data-v-b1004c44] {
  background-color: #e9f0fd;
  font-size: 12px;
  display: flex;
  align-items: center;
  text-align: center;
  font-weight: 400;
  color: #4489fe;
  background: #e9f0fd;
  border: 1px solid #e9f0fd;
  box-sizing: border-box;
  border-radius: 3px;
      min-width: 98px;

}
.add-tag-style {
    width: 85%;
}
.add-tag-style input {
  border: 0;
}
.add-tag-style .form-control:focus {
  box-shadow: none;
  margin: 4px 10px 0;
  padding: 0;
}

.b-form-tags {

  min-height: 122px !important;
    padding: 10px 10px;
    /* background-image: url(assets/i/select-arrow.svg); */
    height: 50px;
    line-height: 28px;
    background-repeat: no-repeat;
    background-position: 90% center;
}

</style>