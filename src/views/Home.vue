<template>
  <div>
    <section class="hero is-medium is-bold">
      <div class="hero-body">
        <div class="container">
          <div class="columns is-vcentered is-centered">
            <div class="column is-5">
              <h1 class="title">{{ $t('message.lead1') }}</h1>
              <h2 class="subtitle">{{ $t('message.lead2') }}</h2>
            </div>
            <div class="column is-narrow">
              <img
                class="image"
                src="../assets/pixel-cells-3976301_1280.png"
                style="width: 400px"
              />
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <div class="columns is-vcentered is-centered">
          <div class="column is-narrow has-text-centered">
            <h2 class="title is-4">{{ $t('heading.video') }}</h2>
            <div style="width: 560px; max-width: 100%">
              <iframe
                width="560"
                height="315"
                style="width: 100%"
                src="https://www.youtube.com/embed/-pAuyU3ZXkU"
                frameborder="0"
                allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen
              ></iframe>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <div class="columns is-vcentered is-centered">
          <div class="column is-narrow has-text-centered">
            <h2 class="title is-4">{{ $t('heading.oss') }}</h2>
            <div>
              <a
                href="https://github.com/project-koudou/koudou-legacy"
                target="_blank"
                class="button"
              >
                <span class="icon" style="margin-right: 5px">
                  <i class="fab fa-github fa-lg"></i>
                </span>
                <span>project-koudou/koudou-legacy</span>
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <div class="columns is-vcentered is-centered">
          <div class="column is-narrow has-text-centered">
            <h2 class="title is-4">{{ $t('heading.pr') }}</h2>
            <div class="content has-text-left">
              <ul>
                <li>
                  <a
                    href="https://medium.com/callforcode/disaster-plans-coded-to-keep-up-in-crisis-2702fea3223f"
                    target="_blank"
                  >
                    Disaster plans coded to keep up in crisis</a
                  >
                  (Call for Code Daily)
                </li>
                <li>
                  <a
                    href="https://web.archive.org/web/20200928181715/https://jp.newsroom.ibm.com/2019-11-14-call-for-code-challenge-2019"
                    target="_blank"
                    >日本IBM、「Call for Code チャレンジ2019」
                    日本最優秀ソリューションを発表</a
                  >
                </li>
                <li>
                  Regional Winner for Japan in
                  <a
                    href="https://web.archive.org/web/20200928181303/https://developer.ibm.com/callforcode/2019-solutions/"
                    target="_blank"
                    >Call for Code 2019 Global Challenge</a
                  >
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          <span>Developed by the KOUDOU Flow team.</span>
          <span>
            “Pixel Cells” illustration by courtesy of
            <a
              href="https://pixabay.com/vectors/pixel-cells-teaching-learn-wiki-3976301/"
              target="_blank"
              >Manfred Steger</a
            >.
          </span>
        </p>
      </div>
    </footer>
  </div>
</template>

<i18n>
{
  "en": {
    "heading": {
      "video": "Video",
      "oss": "Open Source",
      "pr": "Awards & News"
    },
    "message": {
      "lead1": "Preparing for Disasters",
      "lead2": "Plan ahead your actions & get notified in disasters"
    }
  },
  "ja": {
    "heading": {
      "video": "ビデオ",
      "oss": "オープンソース",
      "pr": "受賞・メディア"
    },
    "message": {
      "lead1": "災害に備えよう",
      "lead2": "行動フローを事前に作成・発生時に支援"
    }
  }
}
</i18n>

<script>
export default {
  name: 'home',
  components: {},
};
</script>
