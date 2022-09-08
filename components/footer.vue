<template>
    <div class="footer">
      <div>
        <img src='../assets/hooper/phone.svg' alt="" />
        <p>+993 65 60 88 12</p>
      </div>
      <div>
        <img src="../assets/hooper/mail.svg" alt="" />
        <p>myschool@gmail.com</p>
      </div>
      <div>
        <img src="../assets/hooper/twitter.svg" alt="" />
        <p>#MySchool</p>
      </div>
      <div>
        <img src="../assets/hooper/insta.svg" alt="" />
        <p>@myschool</p>
      </div>
      <div>
        <img src="../assets/hooper/facebook.svg" alt="" />
        <p>myschool</p>
      </div>
      <div>
        <img src="../assets/hooper/linkedin.svg" alt="" />
        <p>myschool</p>
      </div>
    </div>
  </template>
  <style scoped>
  .footer {
    margin: 0 auto;
    width: 1440px;
    background: #057e82;
    padding: 10px 10px;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    margin-top: 40px;
    
  }
  .footer > div {
    display: flex;
    align-items: center;
    width: 26%;
    margin-bottom: 40px;
  }
  .footer > div:nth-child(n + 4) {
    margin-bottom: 0 !important;
  }
  .footer p {
    font-weight: 400;
    font-size: 16px;
    line-height: 18px;
    color: #ffffff;
    margin-left: 20px;
  }
  </style>