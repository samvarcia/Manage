<script>
  import { onMount } from "svelte";

  import Button from "./Button.svelte";
  let Logo = "images/logo.svg";
  let hamburger = "images/icon-hamburger.svg";
  let menu;
  let burger;

  onMount(() => {
    // console.log(menu);
    // console.log(burger);

    // burger.addEventListener("click", hideShow);
    burger.addEventListener("click", function() {
      menu.classList.toggle("is-active");
    });

    // function hideShow() {
    //   if (menu.classList.contains("is-active")) {
    //     menu.classlist.remove("is-active");
    //   } else {
    //     menu.classlist.add("is-active");
    //   }
    // }
  });
</script>

<style>
  .Header {
    font-family: "Be Vietnam", sans-serif;
    width: 100%;
  }
  .Header-container {
    padding: var(--container);
  }
  .Header-content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
  }
  ul {
    display: flex;
    flex-wrap: wrap;
    list-style: none;
  }
  .Header b {
    padding: 0.5rem;
    font-size: 16px;
    cursor: pointer;
  }
  .Header b:hover {
    color: #9d9ea2;
  }
  .burger {
    display: none;
    cursor: pointer;
  }

  @media screen and (max-width: 768px) {
    .Header {
      width: 100% !important;
    }
    .Header-content {
      align-items: inherit;
      justify-content: space-around;
    }
    .Header-container {
      padding: 20px 80px;
    }
    .Header li {
      padding: 15px;
    }
    .Header b {
      font-size: 20px;
    }
    .burger {
      display: block;

      /* padding-left: 200px; */
    }
    .Header-nav ul {
      margin-top: 50px;
      width: 100vw;
      height: 50vh;
      display: flex;
      flex-direction: column;
      position: fixed;
      /* border: 1px solid red; */
      text-align: center;
      background: #fff;
      padding: 0;
      top: 0;
      right: -200vw;
      z-index: 3;
      display: flex;
      justify-content: center;
      align-items: center;
      -webkit-box-shadow: 0px 73px 88px 92px rgba(0, 0, 0, 0.75);
      -moz-box-shadow: 0px 73px 88px 92px rgba(0, 0, 0, 0.75);
      box-shadow: 0px 73px 88px 92px rgba(0, 0, 0, 0.75);
      transition: 0.3s;
    }
    .Header-nav ul.is-active {
      right: 0;
    }
    .bb {
      display: none;
    }
  }
</style>

<div class="Header">
  <div class="Header-container">
    <div class="Header-content">
      <div class="Header-logo">
        <img src={Logo} alt="" />
      </div>

      <div class="Header-nav">
        <ul bind:this={menu} class="menu is-active">
          <li>
            <b>Pricing</b>
          </li>
          <li>
            <b>Product</b>
          </li>
          <li>
            <b>About Us</b>
          </li>
          <li>
            <b>Careers</b>
          </li>
          <li>
            <b>Community</b>
          </li>
        </ul>
      </div>
      <div class="bb">
        <Button />
      </div>
      <i bind:this={burger} class="burger">
        <img src={hamburger} alt="" />
      </i>
    </div>
  </div>
</div>
