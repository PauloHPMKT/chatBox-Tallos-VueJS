<template>
  <div class="box">
    <header class="header">
      <div class="avatar">
        <div class="avatar-pic">
          <img src="img/user.svg" alt="">
        </div>
        <div class="status">
        </div>
      </div>
      <div class="title">
        <h2>
          ChatBot Support
        </h2>
        <span>status</span>
      </div>
    </header>
    <main>
      chatBox
    </main>
    <div class="message-box">
      <input type="text" placeholder="Digite aqui sua mensagem">
      <button>
        <font-awesome-icon :icon="['fas', 'paper-plane']" />
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'chatBox',
}
</script>

<style scoped>
  .box {
    width: 400px;
    height: 600px;
    filter: drop-shadow(-2px -2px 10px rgba(128, 128, 128, 0.685));
    border-radius: 20px;
    background-color: #e9e9e9;
  }

  .header {
    display: flex;
    align-items: center;
    background-color: #009acc;
    color: #fff;
    border-top-left-radius: 20px;
    border-top-right-radius: 20px;
    height: 15%;
    padding: 10px;
  }

  .header .avatar {
    width: 20%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .status {
    width: 13px;
    height: 13px;
    background-color: #00a300;
    border: 0.5px solid #fff;
    border-radius: 100%;
    position: absolute;
    top: 60px;
    left: 60px;
  }

  .avatar-pic {
    background-color: #FFF;
    width: 60px;
    height: 60px;
    border-radius: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 40px;
  }

  .avatar-pic img {
    width: 50px;
  }

  .header .title {
    margin-left: 20px;
    width: 80%;
  }

  .title h2 {
    font-size: 30px;
    font-weight: 500;
  }

  main {
    height: 75%;

  }

  .message-box {
    height: 10%;
    background-clip: #fff;
    border-top: 1px solid rgb(194, 193, 193);
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
    position: relative;
  }

  .message-box input {
    height: 100%;
    width: 85%;
    font-size: 20px;
    padding-left: 15px;
    border: none;
    border-bottom-left-radius: 20px;
    border-bottom-right-radius: 20px;
  }

  .message-box button {
    width: 15%;
    height: 100%;
    background-color: #009acc;
    border: 1px solid #009acc;
    border-radius: 100%;
    font-size: 30px;
    color: #fff;
    position: absolute;
    top: 0;
    cursor: pointer;
  }

  button svg {
    position: absolute;
    top: 12px;
    right: 16px;
  }


</style>