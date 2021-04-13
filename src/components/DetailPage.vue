<template>
  <b-container fluid class="main-container">
    <b-row class="ml-5 justify-content-md-center">
      <b-col class="kucuk-resim-bolum mt-5 ml-5" cols="1">
        <div class="p-1">
          <img
            src="https://cdn-dmod.akinon.net/products/2021/03/25/314204/2e6ee43d-f5a7-466a-8e53-7d8937f63c2c_size90x135_quality90_cropCenter.jpg"
            alt=""
          />
        </div>
        <div class="p-1">
          <img
            src="https://cdn-dmod.akinon.net/products/2021/03/25/314204/ee6a3f3a-ca2f-4ef5-82f7-8d995037bd60_size90x135_quality90_cropCenter.jpg"
            alt=""
          />
        </div>
        <div class="p-1">
          <img
            src="https://cdn-dmod.akinon.net/products/2021/03/25/314203/d4382793-2b45-4d1b-841d-dac6470e8e93_size90x135_quality90_cropCenter.jpg"
            alt=""
          />
        </div>
        <div class="p-1">
          <img
            src="https://cdn-dmod.akinon.net/products/2021/03/25/314204/b20cec1e-d5c2-4b41-ac56-d73d44bf10aa_size90x135_quality90_cropCenter.jpg"
            alt=""
          />
        </div>
        <div class="p-1">
          <img
            src="https://cdn-dmod.akinon.net/products/2021/03/25/314204/2e6ee43d-f5a7-466a-8e53-7d8937f63c2c_size90x135_quality90_cropCenter.jpg"
            alt=""
          />
        </div>
      </b-col>
      <b-col
        class="orta-bolum-buyuk-resim"
        cols="4"
        style="
          flex: 0 0 33.333333% !important;
          max-width: 25.333333% !important;
        "
      >
        <b-card
          img-src="https://cdn-dmod.akinon.net/products/2021/03/25/314204/2e6ee43d-f5a7-466a-8e53-7d8937f63c2c_size670_quality90.jpg"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem"
          class="mb-2 mt-5"
        >
        </b-card>
      </b-col>
      <b-col class="sag-bolum-fiyat-etiket mt-5" cols="6">
        <div class="urun-islemleri">
          <div class="">
            <h4 class="urun-basligi">Pudra Kylie Kadın Deri Ceket</h4>
            <span class="text-muted text-center ml-5 urun-kodu">
              Ürün Kodu: 21SGE5352PR</span
            >
          </div>
          <div class="fiyat-indirim ml-4">
            <span class="text-muted text-center ml-5 indirimsiz-fiyat">1799 TL</span>
            <h2 class="text-success ml-5 fiyat">1099 TL</h2>
            <div class="indirim-yuzde">
              <p>%39</p>
              <span>indirim</span>
              
            </div>
            <div class="secilen-renk">
            <p class="">
              <span class="text-muted">Seçilen Renk:</span>
              <strong>Pudra</strong>
            </p>
            </div>
          </div>
          <div class="kucuk-resim ml-5">
            <img
              src="https://cdn-dmod.akinon.net/products/2021/03/25/314204/2e6ee43d-f5a7-466a-8e53-7d8937f63c2c_size90x135_quality90_cropCenter.jpg"
              alt=""
              class="ml-4 fiyat-alti-resim"
            />
          </div>
          <div class="mt-3 beden-tablosu">
            <a href="#" class="ml-2"
              ><strong
                style="text-decoration: underline; color: black"
                class="ml-5"
                >Beden tablosu</strong
              ></a
            >
          </div>
          <b-col cols="8" class="mt-2 beden-col">
            <b-col class="bedenler">
              <a href="#" class="p-1">XS</a>
              <a href="#" class="p-1">S</a>
              <a href="#" class="p-1">M</a>
              <a href="#" class="p-1">L</a>
              <a href="#" class="p-1">XL</a>
              <a href="#" class="p-1">XSL</a>
              <a href="#" class="p-1">XXXL</a>
            </b-col>
          </b-col>
          <b-col cols="3" class="mt-3 ml-0">
            <div class="adet-secimi">
              <b-form-select
                v-model="selected"
                :options="options"
                class="mb-3 ml-5"
              >
                <!-- This slot appears above the options from 'options' prop -->
                <template #first>
                  <b-form-select-option :value="null"
                    >1 Adet</b-form-select-option
                  >
                </template>
              </b-form-select>
            </div>
          </b-col>
          <b-col cols="6" size="lg">
            <b-button class="sepet-ekle ml-0">Sepete Ekle</b-button>
          </b-col>
          <b-col cols="6" size="lg" class="mt-2">
            <b-button class="fiyat-haberi">FİYAT DÜŞÜNCE HABER VER</b-button>
          </b-col>
          <b-col cols="10">
            <div class="acordion-menu">
            <div class="accordion" role="tablist">
              <div class="mt-2">
                <p block v-b-toggle.accordion-1 class="text-muted">Ürün Bilgileri</p>
              </div>
              <b-collapse
                id="accordion-1"
                accordion="my-accordion"
                role="tabpanel"
              >
                <b-card-body>
                  <b-card-text>{{ text }}</b-card-text>
                </b-card-body>
              </b-collapse>

              <div class="mt-2">
                <p block v-b-toggle.accordion-2 class="text-muted">Taksit Seçenekleri</p>
              </div>
              <b-collapse
                id="accordion-2"
                accordion="my-accordion"
                role="tabpanel"
              >
                <b-card-body>
                  <b-card-text>{{ text }}</b-card-text>
                </b-card-body>
              </b-collapse>

              <div class="mt-2">
                <p block v-b-toggle.accordion-3 class="text-muted">Kargo & Teslimat</p>
              </div>
              <b-collapse
                id="accordion-3"
                accordion="my-accordion"
                role="tabpanel"
              >
                <b-card-body>
                  <b-card-text>{{ kargo }}</b-card-text>
                </b-card-body>
              </b-collapse>
              <div class="mt-2">
                <p block v-b-toggle.accordion-5 class="text-muted">İade, Değişim & İptal</p>
              </div>
              <b-collapse
                id="accordion-5"
                accordion="my-accordion"
                role="tabpanel"
              >
                <b-card-body>
                  <b-card-text>{{ iade }}</b-card-text>
                </b-card-body>
              </b-collapse>
            </div>
            </div>
          </b-col>
          <b-col cols="6" size="lg" class="mt-2 mb-5"
            ><b-button class="fiyat-haberi">Hangi Mağazada Var</b-button></b-col
          >
        </div>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      text: `
         Mükemmel tasarımı ile tarzını ortaya koymak isteyen kadınlara yardımcı olan Kylie kadın deri ceket her yaş grubuna hitap eden özelliklere sahip.
• Üretiminde pearl materyal kullanıldı.
• Deri malzeme ile yapıldı.
• Yakası dik ve zımba detaylı.
• Yan cepleri fermuarlı.
• Göğüs bölümündeki fermuarlı cep farklı bir tarz oluşturuyor. Tarzını Ortaya Koy. Spor tarzın hakim olduğu tasarım ve kesime rağmen birçok farklı giyim tarzı ile rahatlıkla kombin oluşturuyor. Deri ceket tercihini bir yaşam stili olarak belirleyen kadınların alternatifi olmaya devam ediyor.
        `,
      kargo: `
        Saat 16’ya kadar verilen siparişler iş günlerinde 1-3 gün içerisinde kargoya teslim edilir. Resmi tatil günlerinde, Cumartesi ve Pazar günleri de dahil olmak üzere sevkiyat yapılmamaktadır. 250 TL ve üzeri kargo ücretsizdir.
        `,
      iade: `
       İade, Değişim ve İptal sayfamızdaki kurallara uyulması halinde faturanızı göstermek suretiyle tüm alışverişlerinizin değişim işlemlerini Derimod mağazalarından gerçekleştirebilirsiniz Mağazalarımızdan herhangi bir ücret iadesi yapılamamaktadır. İade işlemleri online satış birimimiz tarafından gerçekleştirilmektedir. İade , Değişim ve iptal bölümündeki yönlendirmeleri takip ederek kargo yoluyla iadenizi yapabilirsiniz.`,

      selected: null,
      options: [{ text: "2 Adet" }, { text: "3 Adet" }],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-container {
  position: relative;
  left: 108px;
}
.urun-basligi {
  font-size: 24px;
  color: #000;
  font-weight: 400;
}
.urun-kodu {
  font-size: 12px;
  position: relative;
  left: 35px;
}
.fiyat-indirim {
  margin-left: ;
}
.indirimsiz-fiyat {
  font-size: 11px;
  text-decoration: line-through;
  position: relative;
  left: 75px;
  top: 10px;
  color: #000;
}
.fiyat {
  left: 10px;
  position: relative;
}

.indirim-yuzde {
      position: relative;
    margin-top: -5px;
    margin-left: 10px;
    padding-top: 7px;
    width: 38px;
    height: 35px;
    background-color: #699c31;
    color: #fff;
    font-size: 13px;
    font-weight: 400;
    text-align: center;
    line-height: 1;
    left: 170px;
    top: -40px;
}
.indirim-yuzde > span {
  position: relative;
  top: -18px;
  font-size: 8px;
}
.secilen-renk {
  position: relative;
  left: 65px;
  top: -25px;
  font-weight: 400;
}

.fiyat-alti-resim {
 width: 55px;
 border: 1px solid;
 left: 55px;
 top: -30px;
 position: relative;

}
.beden-tablosu {
  position: relative;
  top: -10px;
  left: 36px;
  font-size: 17px;
  font-weight: 400;
}

.bedenler > a {
  display: inline-block;
  vertical-align: top;
  position: relative;
  margin: 3px;
  padding-top: 9px;
  width: 35px;
  height: 31px;
  font-size: 12px;
  color: #686869;
  text-align: center;
  background-color: #fff;
  border: 1px solid #bababa;
  right: 50px;
}

.adet-secimi {
  position: relative;
  left: 20px;
}


.beden-col {
  margin-left: 20px;
}

.sepet-ekle {
  background-color: black;
  color: #fff;
  margin-top: 10px;
  height: 50px;
  font-weight: 600;
  font-size: 16px;
  text-align: center;
  user-select: none;
  width: 350px;
  position: relative;
  right: 40px;
}
.fiyat-haberi {
  background-color: #fff;
  color: black;
  margin-top: 10px;
  height: 50px;
  font-weight: 600;
  font-size: 16px;
  text-align: center;
  user-select: none;
   width: 350px;
  position: relative;
  right: 40px;
}

.acordion-menu {
  position: relative;
  right: 40px;
}
</style>
