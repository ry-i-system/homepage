<template>
  <div class="contact">
    <p>お問い合わせ・お仕事のご依頼は以下フォームからご連絡ください。翌日以降に折り返しご連絡いたします。</p>
    <br>
    <form action="/sendmail" method="post">
      <div>
        <label for="i_name">お名前</label><br>
        <input id="i_name" type="text" name="name" value="" placeholder="名前 太郎">
      </div>
      <br>
      <div>
        <label for="i_email">メールアドレス</label><br>
        <input id="i_email" type="email" name="email" value="" placeholder="xxxx@xxxx.com">
      </div>
      <br>
      <div>
        <label for="t_message">お問い合わせ内容</label><br>
        <textarea id="t_message" name="message" placeholder="お問い合わせ・お仕事のご依頼はこちらに内容を入力してください。"></textarea>
      </div>
      <br>
      <div class="btn_area">
        <input type="submit" name="btn_confirm" value="送信する" disabled>
      </div>
      <p class="maintenance">※メンテナンス中のため送信できません。</p>
    </form>
  </div>
</template>

<script>
export default {
  name: 'Contact'
}
</script>

<style scoped>
#i_name {
  width: 200px;
}

#i_email {
  width: 300px;
}

#t_message {
  width: 500px;
  height: 200px;
}

.maintenance {
  color:crimson;
}
</style>
