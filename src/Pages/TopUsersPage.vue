<template>
  <header>
    <div class="heading-wrapper">
      <div id="profileSlogan">
        <span>Топ <b>100</b> пользователей</span>
      </div>
    </div>
  </header>
  <!-----------------------------------header----------------------------------------->
  <main>
    <div class="topUsers">
      <a href="#">
        <div class="topUser">
          <div class="userImage">
            <img alt="" src="http://achieve.by:5000/icons/clubs/palace.png" />
          </div>
          <div class="userAboutWrapper">
            <div class="nameSurnameUser">
              <span>First Last</span>
            </div>
            <div class="xpCountUser">
              <span>Опыт: 1000</span>
            </div>
          </div>
          <div class="ClubLogoAndPositionUser">
            <div class="clubUserLogo">
              <img alt="" src="http://achieve.by:5000/icons/clubs/palace.png" />
            </div>
            <div class="topPositionUser">
              <span>#1</span>
            </div>
          </div>
        </div>
      </a>
    </div>
  </main>
</template>

<style scoped>
header {
  background-color: #0e1316;
  border-radius: 0px 0px 50px 50px;
}

main {
  margin-bottom: 3%;
}

.heading-wrapper {
  display: flex;
  justify-content: center;
  padding-top: 15px;
}

#profileSlogan {
  width: 100%;
  font-size: 24px;
  font-family: 'Exo 2', sans-serif;
  font-style: normal;
  font-weight: normal;
  margin: 0;
  color: white;
  text-align: center;
  padding-bottom: 20px;
}

footer {
  width: 100%;
  position: fixed;
  bottom: 0;
}

.footerSections {
  display: flex;
  background: white;
  width: 100%;
  justify-content: center;
  -webkit-box-shadow: 0px -5px 15px 4px rgba(0, 0, 0, 0.2);
  -moz-box-shadow: 0px -5px 15px 4px rgba(0, 0, 0, 0.2);
  box-shadow: 0px -5px 15px 4px rgba(0, 0, 0, 0.2);
}

footer img {
  width: 50px;
  margin: 10px 30px 5px 30px;
  object-fit: cover;
}

.secondSection hr {
  border-bottom: 5px solid #0d4e81;
  border-radius: 10px 10px 0px 0px;
  margin: 0;
}

.topUsers {
  display: flex;
  justify-content: center;
  flex-direction: column;
  margin: 15px;
  align-items: center;
}

.topUsers > a {
  width: 40%;
}

.topUser {
  background: #151e1d;
  border-radius: 20px;
  display: flex;
  padding: 15px;
  margin-top: 15px;
  cursor: pointer;
}

.userImage img {
  width: 50px;
  height: 50px;
  object-fit: cover;
  border-radius: 50%;
}

.userAboutWrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 10px;
  width: 40%;
}

.nameSurnameUser {
  font-family: 'Exo 2';
  font-style: normal;
  font-weight: normal;
  color: white;
}

.xpCountUser {
  font-size: 13px;
  color: white;
}

.xpCountDefaultUser {
  font-size: 13px;
  color: white;
}

.clubUserLogo {
  text-align: center;
  display: flex;
  align-items: center;
  padding-right: 15px;
}

.clubUserLogo img {
  width: 45px;
  object-fit: cover;
}

.topPositionUser {
  font-size: 23px;
  font-weight: bold;
  text-align: center;
  display: flex;
  align-items: center;
  color: white;
}

.topPositionUserDefault {
  font-size: 23px;
  font-weight: normal;
  text-align: center;
  display: flex;
  align-items: center;
  color: white;
}

.ClubLogoAndPositionUser {
  width: 40%;
  display: flex;
  justify-content: flex-end;
}

.px {
  width: 100%;
  height: 75px;
}

@media (max-width: 800px) {
  .topUsers > a {
    width: 80%;
  }

  .topPositionUser {
    font-size: 1.5em;
  }
}

@media (max-width: 430px) {
  #infoTask {
    text-align: left;
  }
}

@media (max-width: 1100px) {
  .ClubLogoAndPositionUser {
    width: 50%;
  }

  .topUsers > a {
    width: 80%;
  }

  .userAboutWrapper {
    width: 50%;
  }

  #infoTask {
    width: 100%;
    text-align: left;
  }

  .notInfoTask {
    width: 100%;
    text-align: left;
  }

  #nameTask {
    text-align: left;
  }

  .aboutTask {
    width: 100%;
  }

  .mark {
    display: unset;
  }

  .taskXP {
    width: 100px;
    text-align: right;
  }

  .completedTask {
    cursor: pointer;
  }

  .notCompletedTask {
    cursor: pointer;
  }
}
</style>
