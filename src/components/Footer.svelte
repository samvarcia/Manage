<script>
  let Logo = "images/WhiteLogo.svg";
  let Insta = "images/icon-instagram.svg";
  let Pint = "images/icon-pinterest.svg";
  let Twit = "images/icon-twitter.svg";
  let You = "images/icon-youtube.svg";
  let Face = "images/icon-facebook.svg";
</script>

<style>
  .Footer-container {
    background-color: hsl(233, 12%, 13%);
    padding: var(--container);
  }
  .Footer-content {
    display: flex;
    flex-wrap: wrap-reverse;
    justify-content: space-around;
  }
  .Footer-media {
    display: flex;
    flex-direction: column;
    justify-content: center;
    flex-wrap: wrap-reverse;
    align-items: space-between;
  }

  .Footer-social ul img {
    padding: 5px;
    margin-top: 70px;
    cursor: pointer;
  }
  .Footer-social ul {
    padding: 0;
  }
  .Footer-links {
    /* border: 1px solid red; */
    color: #fff;
    width: 40%;
    display: flex;
    justify-content: space-between;
  }

  .Footer-links ul li {
    list-style: none;
    padding: 0.5rem;
    cursor: pointer;
  }
  .Footer-links ul li:hover {
    color: var(--main-orange);
  }
  .Input {
    margin-top: 10px;
  }
  .send input {
    border-radius: 30px;
    padding: 10px;
    width: 230px;
  }
  .send button {
    background-color: var(--main-orange);
    border: none;
    color: #fff;
    width: 50px;
    padding: 10px;
    cursor: pointer;
    border-radius: 40px;
  }
  .send button:hover {
    background-color: #f98e75;
    -webkit-box-shadow: 0px 35px 28px -14px rgba(254, 188, 173, 0.8);
    -moz-box-shadow: 0px 35px 28px -14px rgba(254, 188, 173, 0.8);
    box-shadow: 0px 35px 28px -14px rgba(254, 188, 173, 0.8);
  }
  .Input-content p {
    color: var(--main-gray);
  }
  @media screen and (max-width: 768px) {
    .Footer-container {
      padding: 20px 80px;
    }
    .Footer-links ul {
      padding: 0;
    }
    .Footer-links {
      padding: 20px;
      width: 400px;
    }
    .Footer-social ul img {
      margin-top: 40px;
      padding: 10px;
      width: 30px;
    }
  }
</style>

<div class="Footer">
  <div class="Footer-container">
    <div class="Footer-content">
      <div class="Footer-media">
        <img src={Logo} alt="Logo" />
        <div class="Footer-social">
          <ul>
            <img src={Insta} alt="" />
            <img src={Pint} alt="" />
            <img src={Twit} alt="" />
            <img src={You} alt="" />
            <img src={Face} alt="" />
          </ul>
        </div>
      </div>
      <div class="Footer-links">
        <div class="Footer-links-left">
          <ul>
            <li>
              <b>Home</b>
            </li>
            <li>
              <b>Pricing</b>
            </li>
            <li>
              <b>Products</b>
            </li>
            <li>
              <b>About Us</b>
            </li>
          </ul>
        </div>
        <div class="Footer-links-right">
          <ul>
            <li>
              <b>Careers</b>
            </li>
            <li>
              <b>Community</b>
            </li>
            <li>
              <b>Privacy Policy</b>
            </li>
          </ul>
        </div>
      </div>
      <div class="Input">
        <div class="Input-content">
          <div class="send">
            <input type="text" placeholder="Updates in your phone..." />
            <button>Go</button>
          </div>
          <p>Copyright 2020. All rights deserved</p>
        </div>
      </div>
    </div>
  </div>
</div>
