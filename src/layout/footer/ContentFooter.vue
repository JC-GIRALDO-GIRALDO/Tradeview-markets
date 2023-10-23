<script setup>
const socialMediaLogos = [
  {
    name: "Twiter",
    link: "https://twitter.com/Tradeview_",
    logo: "https://i.imgur.com/Lzxt5fE.png",
  },
  {
    name: "Facebook",
    link: "https://www.facebook.com/TradeviewMarkets/",
    logo: "https://i.imgur.com/JesPjPD.png",
  },
  {
    name: "Linkedin",
    link: "https://www.linkedin.com/company/tradeview-forex/",
    logo: "https://i.imgur.com/iKIQLVx.png",
  },
  {
    name: "Instagram",
    link: "https://www.instagram.com/tradeviewmarkets/",
    logo: "https://i.imgur.com/WD02Eg3.png",
  },
  {
    name: "YouTube",
    link: "https://www.youtube.com/@TradeviewMarkets",
    logo: "https://i.imgur.com/zPgIVqd.png",
  },
];
const infoBrands = [
  {
    title: "Tradeview Ltd.",
    info: `Is licensed to carry on securities investment business and is regulated by the
          Cayman Islands Monetary Authority (CIMA) as a full securities broker-dealer. (License
          #585163) Tradeview conducts business pursuant to the Cayman Islands Securities
          Investment Business Law (SIBL) and its activities fall under the direct supervision of
          the Investments and Securities Division of CIMA.`,
    headquarters:
      "Grand Cayman, KY1-1002, 4th Floor Harbour Place | 103 South Church St, PO Box 1105.",
    web: "www.tradeviewforex.com",
  },
  {
    title: "TVM Global Ltd.",
    info: `Is licensed and regulated by the Labuan Financial Services Authority (FSA) as a
          Money Broker, registration number LL15870 licensed to facilitate transactions in
          foreign exchange pursuant to Labuan Financial Services and Securities Act 2010, the
          Labuan Companies Act 1990 and the Labuan Business Activity Tax Act 1990.`,
    headquarters: `International Business Financial Centre at Office 5, Jamie Business
            Center I, Unit F10, First Floor, Paragon Labuan, Jalan Mustapha, 87000 Labuan F.T.`,
    web: "www.tvmgloballtd.com",
  },

  {
    title: "Tradeview Europe Ltd.",
    info: `Is licensed as a Category 2 Investment Service Company and is regulated by the
          Malta Financial Services Authority (MFSA). The Malta Financial Services Authority
          (MFSA) is the single regulator for financial services in Malta. MFSA is a fully
          autonomous public institution and reports to Parliament on an annual basis. The
          MFSA is a member of the European Banking Authority (EBA), the European Securities
          and Markets Authority (ESMA) and the International Organization of Securities
          Commissions (IOSCO) and is a signatory of the Multilateral Memorandum of
          Understanding with other European regulatory Institutions. Tradeview is authorized
          to provide financial services across multiple asset classes and is passported in the
          EU/EEA under MiFID II (EU Markets in Financial Instruments Directive).`,
    headquarters:
      "Grand Cayman, KY1-1002, 4th Floor Harbour Place | 103 South Church St, PO Box 1105.",
    web: "www.tradeviewforex.com",
  },
];
const infoBrandsDos = [
  {
    title: "Tradeview Financial Markets S.A.C Global",
    info: `Is authorized to conduct business pursuant to and in compliance with the General
          Law of Companies (LGS) promulgated by the government of Peru. Tradeview
          Financial Markets S.A.C is registered with the National Superintendence of Public
          Registries (SUNARP), company number 13089531. Tradeview Financial Markets S.A.C
          provides financial services in selected OTC derivative markets in compliance with all
          applicable government regulations.`,
    headquarters: `Los Mirtos 239 Urb. San Eugenio, Lince, Lima, Perú.`,
    web: "www.tradeviewlatam.com",
  },
  {
    title: "iLC Brokers Ltd.",
    info: `iLC Brokers Ltd. is authorized under the Mauritius Financial Service Commission with
          a Global Business License and Investment Dealer License #GB20025800 to provide
          financial services to professional and non-professional clients.`,
    headquarters:
      "6 St. Denis Street, 1/F River Court, Port Louis 11328 Mauritius.",
    web: "www.ilcbrokers.com",
  },
  {
    title: "TVCM Limited (Tradeview UK)",
    info: `Is a limited company registered in England & Wales under Company Number
          08648747 and is authorised and regulated by the Financial Conduct Authority FRN:
          990586`,
    headquarters: `85 Great Portland Street, London W1W 7LT.`,
    web: "www.tradeview.co.uk",
  },
];
</script>

<template>
  <div class="content-footer">
    <div class="content-text-footer">
      <section class="custom-section-1">
        <article class="custom-article-1">
          <div class="contenedor-1">
            <div class="item item-1">
              <img
                src="https://i.imgur.com/fcF9iSV.png"
                alt="logo-gris-empresa"
              />
            </div>
            <div class="item item-2">
              <p>
                <strong class="item-strong">Tradeview Markets</strong> | Grand
                Cayman, KY1-1002, 4th Floor <br />
                Harbour Place | 103 South Church St, PO Box 1105
              </p>
              <p>
                <strong class="item-strong">Main Oﬃce: </strong>+1 345 945 6271
              </p>
              <p>
                <strong class="item-strong">Direct Phone: </strong>+1 345 946
                4532
              </p>
              <p>
                <strong class="item-strong">Website: </strong>
                <u>www.tvmarkets.com</u>
              </p>
            </div>
            <div class="item item-3">
              <p>FIND US ON:</p>
              <div class="socialMediaLogos">
                <img
                  v-for="socialMedia in socialMediaLogos"
                  :key="socialMedia.logo"
                  :src="socialMedia.logo"
                  :alt="socialMedia.name"
                />
              </div>
            </div>
          </div>
          <div class="contenedor-2">
            <div class="item item-4 border p-3 d-flex">
              <div class="coment-surf">
                <div class="content-img-surf">
                  <img src="https://i.imgur.com/UsG6h3d.png" alt="logo-surf" />
                </div>
                <div class="coment-surf-text">
                  <p>
                    Find daily trading insights and understand what is behind
                    the latest waves in financial markets.
                  </p>
                </div>
              </div>
              <div class="d-flex ms-3 surf-input">
                <input
                  type="text"
                  class="form-control bg-transparent me-2"
                  placeholder="Enter your email address"
                />
                <button class="btn btn-primary btn-sm bg-transparent">
                  Subscribe
                </button>
              </div>
            </div>
            <div class="item item-5">
              <div class="link-seccion-item">
                <ul>
                  <li><a href="#">Forex</a></li>
                  <li><a href="#">Stocks</a></li>
                  <li><a href="#">Futures</a></li>
                  <li><a href="#">TradeGATEHUB</a></li>
                  <li><a href="#">Markets</a></li>
                  <li><a href="#">Pricing</a></li>
                  <li><a href="#">Introducing Brokers</a></li>
                  <li><a href="#">Education</a></li>
                  <li><a href="#">Contact US</a></li>
                </ul>
              </div>
              <div class="link-seccion-item-all">
                <ul>
                  ACCOUNTS
                  <li><a href="#">Open account</a></li>
                  <li><a href="#">Individual</a></li>
                  <li><a href="#">Joint</a></li>
                  <li><a href="#">Corporate</a></li>
                </ul>
                <ul>
                  ABOUT TRADEVIEW
                  <li><a href="#">Our Story</a></li>
                  <li><a href="#">Our Team</a></li>
                  <li><a href="#">Our Vision</a></li>
                </ul>
                <ul>
                  COMPANY
                  <li><a href="#">Why Tradeview</a></li>
                  <li><a href="#">Sponsorships</a></li>
                  <li><a href="#">Press</a></li>
                </ul>
              </div>
              <div class="link-seccion-item-all">
                <ul>
                  SOFTWARE
                  <li><a href="#">MetaTrader 4</a></li>
                  <li><a href="#">MetaTrader 5</a></li>
                  <li><a href="#">cTrader</a></li>
                  <li><a href="#">cTrader Copy</a></li>
                  <li><a href="#">Currenex</a></li>
                </ul>
                <ul>
                  SUPPORT
                  <li><a href="#">Forms and Documents</a></li>
                  <li><a href="#">FAQ</a></li>
                </ul>
              </div>
            </div>
          </div>
        </article>
      </section>
      <section class="custom-section-2">
        <article class="custom-article">
          <hr />
          <p>
            <strong
              >IMPORTANT NOTICE TO CLIENTS REGARDING CRYPTO CURRENCY
              PROHIBITION.</strong
            >
            Please be advised that Tradeview Markets does not accept
            cryptocurrency for deposit into client accounts. All deposits to
            client accounts must be made in fiat currency, such as USD, JPY,
            EUR, GBP, CAD and MXN. Clients using third party payment providers
            are prohibited from depositing cryptocurrency into the Tradeview
            Markets account with the third party payment provider and then
            converting the crypto currency to fiat currency for further deposit
            into their account. Tradeview must be able to trace all deposits
            back to a regulated financial institution. Violations of this
            anti-money laundering compliance provision regarding the use of
            crypto currency as a source for deposit into your Tradeview Markets
            account will result in the immediate liquidation of all open
            positions in your account and the permanent closure of your account.
          </p>
          <hr />
          <p>
            There is a risk of loss in trading foreign currencies and it is not
            suitable for everyone. We are compensated for our services through
            the bid-ask spread. Tradeview is not responsible for any gains or
            losses on currency rates or exchanges during any transaction.
            <br />
            Copyright© 2022. All rights reserved.
            <br />
            <br />
            The services and products offered by Tradeview Markets are not being
            offered within the United States (US) and not being oﬀered to US
            Persons, as defined under US law. The information on this website is
            not directed to residents of any country where FX and/or CFDs
            trading is restricted or prohibited by local laws or regulations.
          </p>
          <p>
            <br />
            <strong class="policy">
              Terms and Conditions | Privacy Policy | AML Policy | Withdrawal
              Policy | Refund Policy | Risk Disclosure | FAQ
            </strong>
          </p>
          <hr />
        </article>
      </section>
      <section class="custom-section-3">
        <div class="column">
          <article v-for="brand in infoBrands" :key="brand.title">
            <div class="card">
              <div class="card-body">
                <h5 class="card-title">{{ brand.title }}</h5>
                <p class="card-text">{{ brand.info }}</p>
                <p class="card-text">
                  <strong>Headquarters:</strong> {{ brand.headquarters }}
                </p>
                <a
                  :href="'http://{{brand.web}}'"
                  target="_blank"
                  class="card-link"
                  >Website:<span class="web-brand">{{ brand.web }}</span></a
                >
              </div>
            </div>
          </article>
        </div>
        <div class="column">
          <article v-for="brand in infoBrandsDos" :key="brand.title">
            <div class="card">
              <div class="card-body">
                <h5 class="card-title">{{ brand.title }}</h5>
                <p class="card-text">{{ brand.info }}</p>
                <p class="card-text">
                  <strong>Headquarters:</strong> {{ brand.headquarters }}
                </p>
                <a
                  :href="'http://{{brand.web}}'"
                  target="_blank"
                  class="card-link"
                  >Website:<span class="web-brand">{{ brand.web }}</span></a
                >
              </div>
            </div>
          </article>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped>
.content-footer {
  background-color: #3c3e48;
}
.custom-article-1 {
  margin: 1rem auto;
}
.content-text-footer {
  color: #a2a4aa;
}
.card-link {
  color: #a2a4aa;
}
.policy,
.item-strong {
  color: #f8f8f8;
}
.web-brand {
  color: #f8f8f8;
}
.custom-section-1 {
  display: flex;
  flex-direction: row;
  width: 77%;
  margin: 0 auto;
}
.custom-section-2 {
  display: flex;
  flex-direction: column;
  width: 77%;
  margin: 0 auto;
}
.socialMediaLogos img {
  margin-left: 10px;
  margin-right: 10px;
}
.custom-section-3 {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 80%;
  margin: 0 auto;
}
.custom-article-1 {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.contenedor-1,
.contenedor-2 {
  width: 80%;
  margin-top: 2rem;
}
.item-1 img {
  margin-bottom: 2rem;
}
.item-3 p {
  margin-top: 3rem;
  font-size: 12px;
}
.card-title {
  color: #f8f8f8;
}
.coment-surf {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  padding: 15px;
}
.content-img-surf img {
  width: 150px;
}
.coment-surf-text p {
  margin-left: 50px;
  font-size: 15px;
}
.surf-input {
  margin-top: 1rem;
  margin-bottom: 1rem;
}
.column {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 20px; /* Espacio entre los objetos en la columna */
}
.item-4 {
  display: flex;
  flex-direction: column;
}
.item-5 {
  margin-top: 3rem;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}
.link-seccion-item li {
  margin-bottom: 0.5rem;
  list-style: none;
}
.link-seccion-item a {
  color: #a2a4aa;
}
.link-seccion-item-all ul {
  color: #a2a4aa;
  margin-bottom: 3rem;
}
.link-seccion-item-all li {
  margin-bottom: 0.5rem;
  list-style: none;
}
.link-seccion-item-all a {
  color: #fbfbfb;
  text-decoration: none;
}
.card {
  border: none;
  padding: 10px;
  background-color: transparent;
  color: #a2a4aa;
  line-height: 1;
}
.card-body p {
  margin: 0;
  padding: 0;
}
.card-body h5 {
  margin: 0;
  padding: 0;
}
@media (max-width: 768px) {
  .custom-section-1 {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    margin: 0 auto;
  }
  .custom-section-2 {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    margin: 0 auto;
  }
  .custom-section-3 {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    margin: 0 auto;
  }
  .custom-article-1 {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .custom-article {
    padding: 2rem;
  }
  .contenedor-1,
  .contenedor-2 {
    width: 100%;
    padding: 30px;
  }
  .coment-surf {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .column {
    display: flex;
    flex-direction: column;
  }
  .item-4 {
    display: flex;
    flex-direction: column;
  }
}
</style>
