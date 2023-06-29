<template>
  <main>
    <iframe style="display:none" height="0" width="0" id="loader"></iframe>
    <div class="center-wrapper">
      <div class="main-container">
        <nav>
          <div class="blur-nav"></div>
          <div class="left">
            <button class="downloadButton">
              <picture>
                <source media="(min-width:1125px)" srcset="/assets/images/3x/account@3x.png" width="47" />
                <img src="/assets/images/2x/account@2x.png" width="47">
              </picture>
            </button>
            <picture>
              <source media="(min-width:1125px)" srcset="/assets/images/3x/logo@3x.png" width="86" />
              <img src="/assets/images/2x/logo@2x.png" width="86">
            </picture>
          </div>
          <div class="right relative">
            <button onclick="openLangPanel()">
              <picture>
                <source id="global-lang-pic" media="(min-width:1125px)" srcset="/assets/images/3x/chinese@3x.png"
                  width="20" />
                <img id="global-lang-img" src="/assets/images/2x/chinese@2x.png" width="20">
              </picture>
            </button>
            <div class="btn-selection">
              <button onclick="selectLang(1)"><img src="/assets/images/2x/english@2x.png" width="20" /><span
                  class="lang-icon">English</span></button>
              <button onclick="selectLang(2)"><img src="/assets/images/2x/chinese@2x.png" width="20" /><span
                  class="lang-icon">简体中文</span></button>
              <button onclick="selectLang(3)"><img src="/assets/images/2x/繁體中文@2x.png" width="20" /><span
                  class="lang-icon">繁体中文</span></button>
            </div>
            <button>
              <picture>
                <source media="(min-width:1125px)" srcset="/assets/images/3x/service@3x.png" width="20" />
                <img src="/assets/images/2x/service@2x.png" width="20">
              </picture>
            </button>
          </div>
        </nav>
        <div class="mobile gif-container flex">
          <div class="download-button">
            <button class="download-btn downloadButton">
              <picture>
                <source id="download-btn-pic" media="(min-width:1125px)" srcset="/assets/images/3x/download_cn@3x.png"
                  width="161" />
                <img class="download-btn-img" src="/assets/images/2x/download_cn@2x.png" width="161" />
              </picture>
            </button>
          </div>
          <div class="content">
            <div class="welcome">欢迎来到</div>
            <picture class="metaverse-label">
              <source media="(min-width:1125px)" srcset="/assets/images/3x/asset10@3x.png" width="258" />
              <img src="/assets/images/2x/asset10@2x.png" width="258" />
            </picture>
            <div class="welcome-main-content">世界第一大数据流动性提供商Meta Travers机构，与其一起旅行并赚取被动奖励</div>

            <div class="one-mil">
              <picture>
                <source class="one-mil-pic" media="(min-width:1125px)" srcset="/assets/images/3x/1million_cn@3x.png"
                  width="180" />
                <img class="one-mil-img" src="/assets/images/2x/1million_cn@2x.png" width="180" />
              </picture>
            </div>

            <div class="one-mil-text">MetaTravers 是虚拟和现实旅游行业的大数据流动性提供 商。我们与全球最大的旅游平台密切合作，旨在吸引超过 1000万活跃用户。</div>

            <div class="reward-img">
              <picture>
                <source class="reward-pic" media="(min-width:1125px)" srcset="/assets/images/3x/1billion_cn@3x.png"
                  width="155" />
                <img class="reward-img-id" src="/assets/images/2x/1billion_cn@2x.png" width="155" />
              </picture>
            </div>
            <div class="reward-text">支付总额达10亿用于恢复因 COVID-19 疫情而导致的停摆影响，以建立新的旅游经济生态系统。</div>

            <div class="air-ticket-container">
              <picture>
                <source media="(min-width:1125px)" srcset="/assets/images/3x/asset16@3x.png" width="245" />
                <img src="/assets/images/2x/asset16@2x.png" width="245" />
              </picture>
            </div>
            <div class="air-ticket-text">
              <span class="air-ticket-textspan">Meta Travers向活跃用户赠送了10,000张机票</span>
            </div>

            <div class="opportunity-img">
              <picture>
                <source class="opportunity-sec-pic" media="(min-width:1125px)" src="/assets/images/3x/13000_cn@3x.png"
                  width="260" />
                <img class="opportunity-sec-img" src="/assets/images/2x/13000_cn@2x.png" width="260" />
              </picture>
            </div>
            <div class="opportunity-text">我们的目标是在2019年（疫情之前）8.8万亿美元的旅游 业中创造13,000个商业机会，并培养高收入者。</div>

            <div class="partner-container partner-wrapper-cn">
              <picture>
                <source class="partner-pic" media="(min-width:1125px)" srcset="/assets/images/3x/partners_cn@3x.png"
                  width="240" />
                <img class="partner-img" src="/assets/images/2x/partners_cn@2x.png" width="240" />
              </picture>
            </div>
            <div class="partner-container partner-wrapper-cn-web">
              <div>
                <img class="partner-img" src="/assets/images/3x/战略合作商@3x.png" width="140" />
              </div>
              <div class="partnership-logo">
                <img src="/assets/images/3x/1@3x.png" width="43" />
                <img src="/assets/images/3x/2@3x.png" width="43" />
                <img src="/assets/images/3x/3@3x.png" width="43" />
                <img src="/assets/images/3x/4@3x.png" width="43" />
                <img src="/assets/images/3x/5@3x.png" width="43" />
                <img src="/assets/images/3x/6@3x.png" width="43" />
                <img src="/assets/images/3x/7@3x.png" width="43" />
                <img src="/assets/images/3x/8@3x.png" width="43" />
              </div>
            </div>
          </div>
        </div>

        <div class="btn-selection-web">
          <div class="btn-container-web">
            <button onclick="selectLang(1)"><img src="/assets/images/2x/english@2x.png" width="20" /><span
                class="lang-icon">English</span></button>
            <button onclick="selectLang(2)"><img src="/assets/images/2x/chinese@2x.png" width="20" /><span
                class="lang-icon">简体中文</span></button>
            <button onclick="selectLang(3)"><img src="/assets/images/2x/繁體中文@2x.png" width="20" /><span
                class="lang-icon">繁体中文</span></button>
          </div>
        </div>
        <div class="web gif-container-web flex">
          <div class="canva-container">
            <div class="galaxy">
              <picture>
                <source media="(min-width:1125px)" srcset="/assets/images/3x/银河@3x.png" width="2424" />
                <img src="/assets/images/2x/银河@2x.png" width="808" />
              </picture>
            </div>
            <div class="gyro-canva">
              <canvas id="canvas"></canvas>
            </div>
          </div>
          <div class="content">
            <div class="welcome">欢迎来到</div>
            <picture class="metaverse-label">
              <source media="(min-width:1440px)" srcset="/assets/images/3x/asset10@3x.png" width="400" />
              <img src="/assets/images/3x/asset10@3x.png" width="258" />
              <div class="welcome-main-content">世界第一大数据流动性提供商Meta Travers机构，与其一起旅行并赚取被动奖励</div>

              <div class="download-button">
                <button class="download-btn downloadButton">
                  <img class="download-btn-img" src="/assets/images/3x/download_cn@3x.png" width="180" />
                </button>
              </div>
            </picture>

            <div class="one-mil">
              <picture>
                <source class="one-mil-pic" media="(min-width:1440px)" srcset="/assets/images/3x/1million_cn@3x.png"
                  width="260" />
                <source class="one-mil-pic" media="(min-width:1125px)" srcset="/assets/images/3x/1million_cn@3x.png"
                  width="180" />
                <img class="one-mil-img" src="/assets/images/2x/1million_cn@2x.png" width="180" />
              </picture>
            </div>

            <div class="one-mil-text">MetaTravers 是虚拟和现实旅游行业的大数据流动性提供 商。我们与全球最大的旅游平台密切合作，旨在吸引超过 1000万活跃用户。
            </div>

            <div class="reward-img">
              <picture>
                <source class="reward-pic" media="(min-width:1440px)" srcset="/assets/images/3x/1billion_cn@3x.png"
                  width="200" />
                <source class="reward-pic" media="(min-width:1125px)" srcset="/assets/images/3x/1billion_cn@3x.png"
                  width="155" />
                <img class="reward-img-id" src="/assets/images/2x/1billion_cn@2x.png" width="155" />
              </picture>
            </div>
            <div class="reward-text">支付总额达10亿用于恢复因 COVID-19 疫情而导致的停摆影响，以建立新的旅游经济生态系统。</div>

            <div class="air-ticket-container">
              <picture>
                <source media="(min-width:1125px)" srcset="/assets/images/3x/asset16@3x.png" width="245" />
                <img src="/assets/images/2x/asset16@2x.png" width="245" />
              </picture>
            </div>
            <div class="air-ticket-text">
              <span class="air-ticket-textspan">Meta Travers向活跃用户赠送了10,000张机票</span>
            </div>

            <div class="opportunity-img">
              <picture>
                <source class="opportunity-sec-pic" media="(min-width:1440px)" srcset="/assets/images/3x/13000_cn@3x.png"
                  width="400" />
                <source class="opportunity-sec-pic" media="(min-width:1125px)" src="/assets/images/3x/13000_cn@3x.png"
                  width="260" />
                <img class="opportunity-sec-img" src="/assets/images/2x/13000_cn@2x.png" width="260" />
              </picture>
            </div>
            <div class="opportunity-text">我们的目标是在2019年（疫情之前）8.8万亿美元的旅游 业中创造13,000个商业机会，并培养高收入者。</div>

            <div class="partner-container-web partner-wrapper-cn">
              <picture>
                <source class="partner-pic" media="(min-width:1125px)" srcset="/assets/images/3x/partners_cn@3x.png"
                  width="240" />
                <img class="partner-img" src="/assets/images/2x/partners_cn@2x.png" width="240" />
              </picture>
            </div>
            <div class="partner-container-web partner-wrapper-cn-web">
              <div>
                <picture>
                  <source class="partner-pic-web" media="(min-width:1125px)" srcset="/assets/images/3x/战略合作商@3x.png"
                    width="224" />
                  <img class="partner-img-web" src="/assets/images/2x/战略合作商@2x.png" width="90" />
                </picture>
              </div>
              <div class="partnership-logo">
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/1@3x.png" width="129" />
                  <img src="/assets/images/2x/1@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/2@3x.png" width="129" />
                  <img src="/assets/images/2x/2@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/3@3x.png" width="129" />
                  <img src="/assets/images/2x/3@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/4@3x.png" width="129" />
                  <img src="/assets/images/2x/4@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/4@3x.png" width="129" />
                  <img src="/assets/images/2x/4@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/5@3x.png" width="129" />
                  <img src="/assets/images/2x/5@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/6@3x.png" width="129" />
                  <img src="/assets/images/2x/6@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/7@3x.png" width="129" />
                  <img src="/assets/images/2x/7@2x.png" width="86" />
                </picture>
                <picture>
                  <source media="(min-width:1125px)" srcset="/assets/images/3x/8@3x.png" width="129" />
                  <img src="/assets/images/2x/8@2x.png" width="86" />
                </picture>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="sub-container"></div>
      <div class="footer-container"></div>
    </div>
  </main>
</template>
<script setup>
new OpenInstall({
  /*appKey必选参数，平台为每个应用分配的ID*/
  appKey: "dpz2bf",
  onready: function () {
    var m = this;
    $(".downloadButton").click(function () {
      const isiOS = navigator.userAgent.match('iPad') || navigator.userAgent.match('iPhone') || navigator.userAgent.match('iPod');
      const isAndroid = navigator.userAgent.match('Android');

      let fallbackLink = "https://metatravers.oss-cn-hongkong.aliyuncs.com/app-release.apk";
      // Mobile
      if (isiOS || isAndroid) {
        document.getElementById('loader').src = "dpz2bf://" + window.location.search + window.location.hash;
        fallbackLink = isAndroid ? "https://metatravers.oss-cn-hongkong.aliyuncs.com/app-release.apk" :
          "https://down.ttiossign.com/#/join/6qWlf5";
      }
      window.setTimeout(function () { window.location.replace(fallbackLink); }, 1);
    })
  }
});

let globalLang = "CN";
let device = "mobile";
// fetchApi();

function openLangPanel() {
  const btnEl = document.body.scrollWidth <= 778 ? document.getElementsByClassName("btn-selection")[0] : document.getElementsByClassName("btn-container-web")[0];
  const type = {
    0: "EN",
    1: "CN",
    2: "TW"
  };
  Array.from(btnEl.children).forEach(element => {
    const type = {
      English: "EN",
      简体中文: "CN",
      繁体中文: "TW"
    };
    if (globalLang === type[element.textContent]) {
      console.log('e', element.textContent);
      element.style.display = "none";
    } else {
      element.style.display = "flex";
    }
  });
  btnEl.classList.add("lang-icon-container");
}

function getLangOpt() {
  const type = {
    "EN": 0,
    "CN": 1,
    "TW": 2
  };
  return type[globalLang];
}

function selectLang(type) {
  const langObj = {
    1: "EN",
    2: "CN",
    3: "TW"
  };
  globalLang = langObj[type];
  changeLanguage(type);
  const btnEl = document.body.scrollWidth <= 778 ? document.getElementsByClassName("btn-selection")[0] : document.getElementsByClassName("btn-container-web")[0];
  btnEl.classList.remove("lang-icon-container");
}

function changeLanguage(type) {
  let globalLangPicIcon = document.getElementById("global-lang-pic");
  const globalLangPicIconObj = {
    1: "/assets/images/3x/english@3x.png",
    2: "/assets/images/3x/chinese@3x.png",
    3: "/assets/images/3x/繁體中文@3x.png"
  };
  globalLangPicIcon.srcset = globalLangPicIconObj[type];

  let globalLangImgIcon = document.getElementById("global-lang-img");
  const globalLangImgIconObj = {
    1: "/assets/images/2x/english@2x.png",
    2: "/assets/images/2x/chinese@2x.png",
    3: "/assets/images/2x/繁體中文@2x.png"
  };
  globalLangImgIcon.src = globalLangImgIconObj[type];

  let downloadBtnPicIcon = document.getElementById("download-btn-pic");
  const downloadBtnPicIconObj = {
    1: "/assets/images/3x/download@3x.png",
    2: "/assets/images/3x/download_cn@3x.png",
    3: "/assets/images/3x/下载按钮-繁體@3x.png"
  };
  downloadBtnPicIcon.srcset = downloadBtnPicIconObj[type];

  let downloadBtnImgIcon = document.getElementsByClassName("download-btn-img");
  const downloadBtnImgIconObj = {
    1: "/assets/images/2x/download@2x.png",
    2: "/assets/images/2x/download_cn@2x.png",
    3: "/assets/images/2x/下载按钮-繁體@2x.png"
  };
  downloadBtnImgIcon[0].src = downloadBtnImgIconObj[type];
  downloadBtnImgIcon[1].src = downloadBtnImgIconObj[type];

  let welcomeLabel = document.querySelectorAll(".welcome");
  const welcomeLabelObj = {
    1: "WELCOME TO",
    2: "欢迎来到",
    3: "歡迎來到"
  };
  welcomeLabel[0].textContent = welcomeLabelObj[type];
  welcomeLabel[1].textContent = welcomeLabelObj[type];

  let welcomeMainContent = document.querySelectorAll(".welcome-main-content");
  const welcomeMainContentObj = {
    1: "AGENCY world’s No1 Big Data Liquidity Provider TRAVEL & EARN with Meta Travers and build passive rewards",
    2: "世界第一大数据流动性提供商Meta Travers机构，与其一起旅行并赚取被动奖励",
    3: "世界第一大數據流動性提供商Meta Travers機構，與其一起旅行並賺取被動獎勵"
  };
  welcomeMainContent[0].textContent = welcomeMainContentObj[type];
  welcomeMainContent[1].textContent = welcomeMainContentObj[type];

  let oneMilPic = document.getElementsByClassName("one-mil-pic");
  const oneMilPicObj = {
    1: "/assets/images/3x/1million@3x.png",
    2: "/assets/images/3x/1million_cn@3x.png",
    3: "/assets/images/3x/100万@3x.png"
  };
  oneMilPic[0].srcset = oneMilPicObj[type];
  oneMilPic[1].srcset = oneMilPicObj[type];
  oneMilPic[2].srcset = oneMilPicObj[type];

  let oneMilImg = document.getElementsByClassName("one-mil-img");
  const oneMilImgObj = {
    1: "/assets/images/2x/1million@2x.png",
    2: "/assets/images/2x/1million_cn@2x.png",
    3: "/assets/images/2x/100万@2x.png",
  }
  oneMilImg[0].src = oneMilImgObj[type];
  oneMilImg[1].src = oneMilImgObj[type];

  if (document.body.scrollWidth > 768) {
    const oneMilWidthObj = {
      1: "280px",
      2: "240px",
      3: "240px",
    }
    oneMilPic[0].style.width = oneMilWidthObj[type];
    oneMilPic[1].style.width = oneMilWidthObj[type];
    oneMilPic[2].style.width = oneMilWidthObj[type];
    oneMilImg[0].style.width = oneMilWidthObj[type];
    oneMilImg[1].style.width = oneMilWidthObj[type];
  }

  let oneMilLabel = document.querySelectorAll(".one-mil-text");
  const oneMilLabelObj = {
    1: "Metatravers is a big Data Liquidity Provider for Tourism &Travelling lndustries in Virtual & Reality. We working close with the largest travel platform the world to build more than 10 million active users.",
    2: "MetaTravers 是虚拟和现实旅游行业的大数据流动性提供 商。我们与全球最大的旅游平台密切合作，旨在吸引超过 1000万活跃用户。",
    3: "MetaTravers 是虛擬和現實旅遊行業的大數據流動性提供 商。我們與全球最大的旅遊平台密切合作，旨在吸引超過 1000萬活躍用戶。"
  }
  oneMilLabel[0].textContent = oneMilLabelObj[type];
  oneMilLabel[1].textContent = oneMilLabelObj[type];

  let rewardPic = document.getElementsByClassName("reward-pic");
  const rewardPicObj = {
    1: "/assets/images/3x/1billion@3x.png",
    2: "/assets/images/3x/1billion_cn@3x.png",
    3: "/assets/images/3x/10亿@3x.png"
  };
  rewardPic[0].srcset = rewardPicObj[type];
  rewardPic[1].srcset = rewardPicObj[type];
  rewardPic[2].srcset = rewardPicObj[type];

  let rewardImg = document.getElementsByClassName("reward-img-id");
  const rewardImgObj = {
    1: "/assets/images/2x/1billion@2x.png",
    2: "/assets/images/2x/1billion_cn@2x.png",
    3: "/assets/images/2x/10亿@2x.png",
  };
  rewardImg[0].src = rewardImgObj[type];
  rewardImg[1].src = rewardImgObj[type];

  const rewardStyle = {
    1: "240px",
    2: "155px",
    3: "155px"
  };

  rewardPic[0].style.width = rewardStyle[type];
  rewardPic[1].style.width = rewardStyle[type];
  rewardImg[0].style.width = rewardStyle[type];
  rewardImg[1].style.width = rewardStyle[type];

  const rewardWebStyle = {
    1: "340px",
    2: "220px",
    3: "200px",
  }
  if (document.body.scrollWidth > 768) {
    rewardPic[0].style.width = rewardWebStyle[type];
    rewardPic[1].style.width = rewardWebStyle[type];
    rewardPic[2].style.width = rewardWebStyle[type];
    rewardImg[0].style.width = rewardWebStyle[type];
    rewardImg[1].style.width = rewardWebStyle[type];
  }


  let rewardLabel = document.querySelectorAll(".reward-text");
  rewardLabelObj = {
    1: "1 Billion total payment to recover the downtime of the covid - 19.Impact to the tourism industries, build new economic ecosystem.",
    2: "支付总额达10亿用于恢复因 COVID-19 疫情而导致的停摆影响，以建立新的旅游经济生态系统。",
    3: "支付總額達10億用於恢復因 COVID-19 疫情而導致的停擺影響，以建立新的旅遊經濟生態系統。"
  };
  rewardLabel[0].textContent = rewardLabelObj[type];
  rewardLabel[1].textContent = rewardLabelObj[type];

  let airTicketLabel = document.getElementsByClassName("air-ticket-textspan");
  const airTicketLabelObj = {
    1: "Meta Travers give away 10,000 Air tickets to the Active Users",
    2: "Meta Travers向活跃用户赠送了10,000张机票",
    3: "Meta Travers向活躍用戶贈送了10,000張機票",
  };
  airTicketLabel[0].textContent = airTicketLabelObj[type];
  airTicketLabel[1].textContent = airTicketLabelObj[type];

  let opportunityPic = document.getElementsByClassName("opportunity-sec-pic");
  const opportunityPicObj = {
    1: document.body.scrollWidth <= 778 ? "/assets/images/3x/13000@3x.png" : "/assets/images/3x/13000_web@3x.png",
    2: "/assets/images/3x/13000_cn@3x.png",
    3: "/assets/images/3x/13000个@3x.png"
  };
  opportunityPic[0].srcset = opportunityPicObj[type];
  opportunityPic[1].srcset = opportunityPicObj[type];
  opportunityPic[2].srcset = opportunityPicObj[type];

  let opportunityImg = document.getElementsByClassName("opportunity-sec-img");
  const opportunityImgObj = {
    1: document.body.scrollWidth <= 778 ? "/assets/images/2x/13000@2x.png" : "/assets/images/2x/13000_web@2x.png",
    2: "/assets/images/2x/13000_cn@2x.png",
    3: "/assets/images/2x/13000个@2x.png"
  };
  opportunityImg[0].src = opportunityImgObj[type];
  opportunityImg[1].src = opportunityImgObj[type];

  const opportunityStyle = {
    1: document.body.scrollWidth <= 778 ? "240px" : "500px",
    2: "508px",
    3: document.body.scrollWidth <= 778 ? "260px" : "400px"
  }
  opportunityPic[0].style.width = opportunityStyle[type];
  opportunityPic[1].style.width = opportunityStyle[type];
  opportunityPic[2].style.width = opportunityStyle[type];
  opportunityImg[0].style.width = opportunityStyle[type];
  opportunityImg[1].style.width = opportunityStyle[type];

  let opportunityLabel = document.querySelectorAll(".opportunity-text");
  const opportunityLabelObj = {
    1: "Our goals to create 13,000 business opportunities and build high lncome earner in the $8.8 trillion travelling industries at 2019 (Before Pendemic)",
    2: "我们的目标是在2019年（疫情之前）8.8万亿美元的旅游 业中创造13,000个商业机会，并培养高收入者。",
    3: "我們的目標是在2019年（疫情之前）8.8萬億美元的旅遊 業中創造13,000個商業機會，並培養高收入者。"
  };
  opportunityLabel[0].textContent = opportunityLabelObj[type];
  opportunityLabel[1].textContent = opportunityLabelObj[type];

  let partnerContainer = document.getElementsByClassName("partner-container");
  if (["CN", "TW"].includes(globalLang)) {
    partnerContainer[0].classList.add("partner-wrapper-cn");
    partnerContainer[1].classList.add("partner-wrapper-cn");
    partnerContainer[0].classList.remove("partner-wrapper-en");
    partnerContainer[1].classList.remove("partner-wrapper-en");
  } else {
    partnerContainer[0].classList.add("partner-wrapper-en");
    partnerContainer[1].classList.add("partner-wrapper-en");
    partnerContainer[0].classList.remove("partner-wrapper-cn");
    partnerContainer[1].classList.remove("partner-wrapper-cn");
  }

  let partnerPic = document.getElementsByClassName("partner-pic");
  const partnerPicObj = {
    1: "/assets/images/3x/partners@3x.png",
    2: "/assets/images/3x/partners_cn@3x.png",
    3: "/assets/images/3x/合作商@3x.png"
  };
  partnerPic[0].srcset = partnerPicObj[type];
  partnerPic[1].srcset = partnerPicObj[type];

  let partnerImg = document.getElementsByClassName("partner-img");
  const partnerImgObj = {
    1: "/assets/images/2x/partners@2x.png",
    2: "/assets/images/2x/partners_cn@2x.png",
    3: "/assets/images/2x/合作商@2x.png"
  };
  partnerImg[0].src = partnerImgObj[type];

  let partnerPicWeb = document.getElementsByClassName("partner-pic-web");
  const partnerPicWebObj = {
    1: "/assets/images/3x/战略合作商-英文@3x.png",
    2: "/assets/images/3x/战略合作商@3x.png",
    3: "/assets/images/3x/战略合作商_web@3x.png"
  }
  partnerPicWeb[0].srcset = partnerPicWebObj[type];

  let partnerImgWeb = document.getElementsByClassName("partner-img-web");
  const partnerImgWebObj = {
    1: "/assets/images/2x/战略合作商-英文@2x.png",
    2: "/assets/images/2x/战略合作商@2x.png",
    3: "/assets/images/2x/战略合作商_web@2x.png"
  };
  const partnerImgWebWidthObj = {
    1: "340px",
    2: "200px",
    3: "200px"
  };
  partnerImgWeb[0].src = partnerImgWebObj[type];
  partnerImgWeb[0].style.width = partnerImgWebWidthObj[type];
  partnerPicWeb[0].style.width = partnerPicWebObj[type];
}

function getOS() {
  const isiOS = /iPad|iPhone|iPod/.test(navigator.userAgent) && !window.MSStream;
  if (isiOS) return "ios";
  return "android";
}

        // async function fetchApi() {
        //     const requestOpts = {
        //         method: "POST",
        //         headers: { 'Content-Type': 'application/json' },
        //         body: JSON.stringify({
        //             type: this.getOS()
        //         })
        //     };
        //     fetch(`${window.location.origin}/api/common/version`, requestOpts)
        //         .then(res => res.json())
        //         .then(res => {
        //             if (res && res.data) {
        //                 let downloadBtn = document.getElementById("download-btn");
        //                 downloadBtn.href = res.data?.link;
        //             }
        //         });
        // }
</script>
