<script setup lang="ts">
import AppSidebar from './AppSidebar.vue'
import ContentTiles from './ContentTiles.vue'
import ContentTile from './ContentTile.vue'
</script>

<template>
  <div class="content-wrapper">
    <app-sidebar />

    <div class="content-area">
      <content-tiles title="Popular Artists">
        <template #tilesWrapper>
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616100005174cb6926f44f620555ba444fca"
            title="Pritam"
            subTitle="Artist"
            tileType="circle"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616100005174cb6926f44f620555ba444fca"
            title="Pritam"
            subTitle="Artist"
            tileType="circle"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616100005174cb6926f44f620555ba444fca"
            title="Pritam"
            subTitle="Artist"
            tileType="circle"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616100005174cb6926f44f620555ba444fca"
            title="Pritam"
            subTitle="Artist"
            tileType="circle"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616100005174cb6926f44f620555ba444fca"
            title="Pritam"
            subTitle="Artist"
            tileType="circle"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616100005174cb6926f44f620555ba444fca"
            title="Pritam"
            subTitle="Artist"
            tileType="circle"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616100005174cb6926f44f620555ba444fca"
            title="Pritam"
            subTitle="Artist"
            tileType="circle"
          />
        </template>
      </content-tiles>

      <content-tiles title="Popular Albums and Singles">
        <template #tilesWrapper>
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616d00001e02e46e7c9f477b2bc0c41688c8"
            title="Pritam"
            subTitle="Artist"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616d00001e02e46e7c9f477b2bc0c41688c8"
            title="Pritam"
            subTitle="Artist"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616d00001e02e46e7c9f477b2bc0c41688c8"
            title="Pritam"
            subTitle="Artist"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616d00001e02e46e7c9f477b2bc0c41688c8"
            title="Pritam"
            subTitle="Artist"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616d00001e02e46e7c9f477b2bc0c41688c8"
            title="Pritam"
            subTitle="Artist"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616d00001e02e46e7c9f477b2bc0c41688c8"
            title="Pritam"
            subTitle="Artist"
          />
          <content-tile
            imgSrc="https://i.scdn.co/image/ab67616d00001e02e46e7c9f477b2bc0c41688c8"
            title="Pritam"
            subTitle="Artist"
          />
        </template>
      </content-tiles>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use '@/assets/scss/variables' as vars;

.content-wrapper {
  padding-inline: 8px;
  padding-block-end: 8px;
  flex-grow: 1;
  display: flex;
  gap: 8px;
}

.content-area {
  flex-grow: 1;
  background: vars.color(lesser-dark);
  border-radius: 8px;
  padding-inline: 16px;
}
</style>
