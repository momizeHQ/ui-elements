<template>
  <div class="notification-wraper">
    <h6>Notifications</h6>
    <a href="#" class="dropdown-item d-flex align-items-center">
      <div class="notify-icon">
        <div class="icon-circle bg-primary">
          <i class="fas fa-file-alt text-white" aria-hidden="true"></i>
        </div>
      </div>
      <div class="main-notify">
        <div class="notify-date">13 July 2021</div>
        <span>
          A new monthly report is ready to download!
        </span>
      </div>
    </a>
  </div>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>

.notification-wraper {
  position: fixed;
  margin-top: 1em;
  margin-left: .5em;
  margin-right: .5em;
  left: 0;
  background-color: #fff;
  box-shadow: 0 0.15rem 1.75rem 0 rgb(58 59 69 / 15%) !important;
}


.notification-wraper h6 {
  background-color: #090963;
  border: 1px solid #090963;
  padding: 0.75rem 1em;
  color: #fff;
  border-top-right-radius: 0.35rem;
  border-top-left-radius: 0.35rem;
  text-transform: uppercase;
  font-weight: 700;
}

.notify-icon{
    margin-right: .75rem;
}

.icon-circle{
    height: 2.5rem;
    width: 2.5rem;
    border-radius: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.main-notify{
    text-align: left;
}

.main-notify .notify-date{
    font-weight: 400;
    font-size: 80%;
    color: #b7b9cc;
}

.main-notify span{
    font-weight: 600;
}

@media (min-width: 540px) {
    .notification-wraper {
        position: absolute;
        right: 0;
        background-color: #fff;
        z-index: 1000;
        border-radius: 0.35rem;
        left: auto;
    }

}

@media (max-width: 530px) {
    .main-notify{
        background: border-box;
        white-space: normal;
    }
}

</style>
