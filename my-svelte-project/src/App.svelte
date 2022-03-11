<script>
  import MyFooter from "./MyFooter.svelte";
  import MyButton from "./MyButton.svelte";
  import Badge from "./Badge.svelte";
  import Card from "./Card.svelte";
  import Avatar from "./Avatar.svelte";

  import ButtonwBadge from "./ButtonwBadge.svelte";
</script>

<body>
  <main>
    <div class="titel">
      <h1>Mine komponenter</h1>
    </div>
    <section class="badges">
      <div>
        <h2>Badges</h2>
      </div>
      <article>
        <Badge type="neutral" title="neutral" />
        <pre><code>{'<Badge type="neutral" title="neutral"/>'}</code></pre>
      </article>
      <article>
        <Badge type="primary" title="primary" />
        <pre><code>{'<Badge type="primary" title="primary"/>'}</code></pre>
      </article>
      <article>
        <Badge type="secondary" title="secondary" />
        <pre><code>{'<Badge type="secondary" title="secondary"/>'}</code></pre>
      </article>
      <article>
        <Badge type="accent" title="accent" />
        <pre><code>{' <Badge type="accent" title="accent"/>'}</code></pre>
      </article>
      <article>
        <Badge type="ghost" title="ghost" />
        <pre><code>{'<Badge type="ghost" title="ghost"/>'}</code></pre>
      </article>
    </section>

    <section class="buttons">
      <div>
        <h2>Knapper</h2>
      </div>
      <article>
        <MyButton type="primary">Først Knap</MyButton>
        <pre><code>{'<MyButton type="primary">Først Knap</MyButton>'}</code
          ></pre>
      </article>
      <article>
        <MyButton type="secondary">Anden Knap</MyButton>
        <pre><code>{'<MyButton type="secondary">Anden Knap</MyButton>'}</code
          ></pre>
      </article>
      <article>
        <MyButton type="accent">Accent</MyButton>
        <pre><code>{'<MyButton type="accent">Accent</MyButton>'}</code></pre>
      </article>
      <article>
        <MyButton type="ghost">Ghost</MyButton>
        <pre><code>{' <MyButton type="ghost">Ghost</MyButton>'}</code></pre>
      </article>
      <article>
        <MyButton type="link">Link</MyButton>
        <pre><code>{'<MyButton type="link">Link</MyButton>'}</code></pre>
      </article>
    </section>

    <section class="cards">
      <div>
        <h2>Kort</h2>
      </div>
      <article>
        <Card />
        <pre><code> {"<Card />"} </code></pre>
      </article>
    </section>

    <section class="button-w-badge">
      <div>
        <h2>Knap m. badge</h2>
      </div>
      <article>
        <ButtonwBadge />
        <pre><code> {"<ButtonwBadge/>"} </code></pre>
      </article>
    </section>

    <section class="avatar">
      <div>
        <h2>Avatar</h2>
      </div>
      <article>
        <Avatar initial="LF" size="mainCircle" />
        <pre><code> &lt; Avatar initial="LF" size="mainCircle" /&gt; </code></pre>
      </article>
      <article>
        <Avatar initial="LF" size="mainCircleMedium" mode="indikator" />
        <pre><code> &lt; Avatar initial="LF" 
        size="mainCircleMedium" mode="indikator /&gt; </code></pre>
      </article>
      <article>
        <Avatar initial="LF" size="mainCircleSmall" />
        <pre><code> &lt; Avatar initial="LF" size="mainCircleSmall" /&gt; </code></pre>
      </article>
    </section>

    <div class="footerSection">
      <div>
        <h2>Footer</h2>
      </div>
      <article>
        <pre><code> {"<MyFooter />"}</code></pre>
      </article>
    </div>
    <MyFooter />
  </main>
</body>

<style>
  .titel {
    border-bottom: solid black 2px;
  }

  article {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background: rgb(240, 239, 239);
    padding: 2rem;
    border-radius: 8px;
    width: 500px;
  }

  @media only screen and (max-width: 600px) {
    article {
      width: 300px;
    }
  }

  pre {
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 8px;
    height: 2rem;
    padding: 0.5rem;
    background-color: rgb(49, 49, 49);
  }
</style>
