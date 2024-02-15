 <template>
  <div class = "user-container">
      <div>
        <i class="fa-sharp fa-solid fa-user"></i>
      </div>
      <div class="user-description">
        <!-- 등록하는 영역에서 작성 -->
        <slot name="item-one"></slot>
      <div class="time">
        <slot name="item-two"></slot>
        sda
      </div>
    </div>
  </div>

   
</template>

<script>
export default {
}
</script>

<style scoped>
.user-container {
  display: flex;
  align-items: center;
  padding: 0.5rem;

}
.fa-user {
  font-size: 2.5rem
}
.user-description {
  padding-left: 8px;
}
.time {
  font-size: 0.7rem;
}
</style>