<template>
  <!-- HEADER -->
  <nav>
    <p class="bigFont">MemeHistory</p>
    <p @click="togglePage('blog');">Home</p>
    <p @click="togglePage('popular');">Popular</p>
    <p @click="togglePage('weather');">Weather</p>
  </nav>



  <div>
    <!-- HOME -->
    <div class="home" v-if="pageActive.blog">

      <div class="homeContents">
        
        <!--Title-->
        <h1 class="bigFont pageTitle">Blog</h1>

        <!--Blogs-->
        <div class="blogSection homeBlog">

          <div>
            <img src="https://e3.365dm.com/19/09/2048x1152/skynews-drew-scanlon-blinking-white-guy_4786055.jpg" alt="WhiteGuyBlinkingMeme" class="blogImg" @click="toggleActualBlog('page1')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page1')">White guy blinking meme</h1>
            <p class="blogDate"><i>posted on</i> Dec 28th 2023</p>
            <p class="blogDesc">
              The White Guy Blinking meme features Drew Scanlon, a video producer, reacting with a surprised blink during a 2013 Giant Bomb live stream. His reaction to an unexpected comment resurfaced in 2017, becoming a viral meme used to express disbelief or confusion. Its simplicity made it a popular and enduring reaction meme online.
            </p>
          </div>

          <div>
            <img src="https://i.insider.com/601448566dfbe10018e00c5d?width=700" alt="StonksMeme" class="blogImg" @click="toggleActualBlog('page2')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page2')">Stonks meme</h1>
            <p class="blogDate"><i>posted on</i> Dec 23rd 2013</p>
            <p class="blogDesc">
              The Stonks meme originated from a 2017 Facebook post by the surrealist meme page Special Meme Fresh, featuring a 3D character known as "Meme Man" standing in front of a graph with the misspelled word "stonks" instead of "stocks." The meme humorously represents poor financial decisions or misunderstood concepts in economics and investing. Its absurdity and visual simplicity made it a popular and widely shared meme across the internet.
            </p>
          </div>

          <div>
            <img src="https://cache.lahelu.com/image-P0Rv0PSAo-92805" alt="WaduhMeme" class="blogImg" @click="toggleActualBlog('page3')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page3')">Waduh meme</h1>
            <p class="blogDate"><i>posted on</i> Jan 18th 2023</p>
            <p class="blogDesc">
              The "Waduh" meme originates from a viral video of a person named Wicaksono, who in a 2017 Indonesian video, exclaims "Waduh" with a mix of surprise and frustration when encountering a minor inconvenience. The clip, with its expressive reaction and distinctive use of the word "waduh," quickly gained traction online, becoming a popular meme format for conveying exaggerated surprise or dismay. Its simple and relatable expression of mild annoyance made it a favorite for various humorous contexts on social media.
            </p>
          </div>

          <div>
            <img src="https://upload.wikimedia.org/wikipedia/en/f/ff/SuccessKid.jpg" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page4')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page4')">Success kid meme</h1>
            <p class="blogDate"><i>posted on</i> Jun 10th 2022</p>
            <p class="blogDesc">
              The Success Kid meme features a photo of a young boy named Sammy Griner clenching his fist with a determined expression, originally taken by his mother in 2007 at the beach. The image gained viral popularity as it was widely used to symbolize small victories and personal triumphs, often accompanied by humorous or inspirational captions. Its widespread appeal and versatility made it one of the most enduring and recognizable memes on the internet.
            </p>
          </div>

          <div>
            <img src="https://uploads.dailydot.com/2023/10/Shocked-Meme.jpg?auto=compress&fm=pjpg" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page5')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page5')">Shocked black guy meme</h1>
            <p class="blogDate"><i>posted on</i> Aug 20th 2015</p>
            <p class="blogDesc">
              The Shocked Black Guy meme features a still image of a man named Tariq Nasheed from a 2009 YouTube video, where he displays a wide-eyed, shocked expression. The image gained popularity as a reaction meme to convey surprise, disbelief, or shock in response to unexpected or dramatic statements. Its exaggerated expression and context made it a widely recognizable and versatile meme on social media.
            </p>
          </div>

        </div>

        <!-- PAGES -->
        <button @click="togglePage('blog')">2</button>
        <button @click="togglePage('blogTwo')">1</button>
        
      </div>

      <div class="homeAds">
        
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSXzd7TCMT-ZrQojI2IGRrEHd9Kn_symsTK6A&s" alt="advertisement">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbwqWgTO2ax1zw-PEjUsLqLKOFJb8Jft7D4g&s" alt="advertisement">
        <img src="https://pbs.twimg.com/media/Dt8ebcyW0AAG0ya?format=jpg&name=4096x4096" alt="advertisement">

      </div>

    </div>

    <!-- 2ND HOME PAGE -->
    <div class="home" v-if="pageActive.blogTwo">

      <div class="homeContents">

        <!--Blogs-->
        <div class="blogSection homeBlog">

          <div>
            <img src="https://i.kym-cdn.com/entries/icons/facebook/000/027/475/Screen_Shot_2018-10-25_at_11.02.15_AM.jpg" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page6')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page6')">Surprised pikachu meme</h1>
            <p class="blogDate"><i>posted on</i> Feb 13th 2008</p>
            <p class="blogDesc">
              The Surprised Pikachu meme originates from a scene in the Pokémon animated series where Pikachu displays a shocked and surprised expression. This reaction shot became popular on the internet as a way to humorously illustrate instances where someone is caught off guard by predictable outcomes or their own mistakes. Its simplicity and expressive nature made it a widely recognized and versatile meme.
            </p>
          </div>

          <div>
            <img src="https://us-tuna-sounds-images.voicemod.net/e54c6d53-6c5d-47e3-9feb-6dc0d22437e1-1702824730148.jpg" alt="StonksMeme" class="blogImg" @click="toggleActualBlog('page7')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page7')">The rock eyebrow meme</h1>
            <p class="blogDate"><i>posted on</i> Apr 3rd 2013</p>
            <p class="blogDesc">
              The Rock Eyebrow meme features a still image of Dwayne "The Rock" Johnson raising one eyebrow in a distinctive, expressive manner. The image is often used online to convey skepticism, curiosity, or surprise, playing on Johnson's iconic and charismatic facial expression. Its widespread appeal stems from The Rock's well-known persona and the meme's versatility in expressing a range of reactions.
            </p>
          </div>

          <div>
            <img src="https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2019/11/01-Confused-Nick-Young-Meme.png" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page8')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page8')">Confused meme</h1>
            <p class="blogDate"><i>posted on</i> Feb 18th 2033</p>
            <p class="blogDesc">
              The Confused meme features an image of a man with a perplexed expression, often used to represent confusion or disorientation. The meme typically shows the man in a state of bewilderment, making it a popular choice for illustrating moments when something doesn’t quite make sense. Its humorous portrayal of confusion resonates with many, making it a widely shared and adaptable meme format.
            </p>
          </div>

          <div>
            <img src="https://pbs.twimg.com/media/FrmIRCcagAIdvhW.jpg" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page9')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page9')">Biar apa? biarin meme</h1>
            <p class="blogDate"><i>posted on</i> Aug 17th 1945</p>
            <p class="blogDesc">
              The "Biar apa? Biarin" meme originates from an Indonesian video where a man, humorously and nonchalantly, responds to a question with "Biar apa? Biarin," which translates to "Why? Just let it be." The phrase is used to convey a laid-back, indifferent attitude toward problems or challenges, often highlighting a humorous or relaxed approach to situations. The meme gained popularity for its relatable and carefree message, resonating widely with audiences who appreciate its easygoing humor.
            </p>
          </div>

          <div>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQv7YsjKKlyiMikvRYW8fxYuXLVO8jEM3X45Q&s" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page10')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page10')">Mike Wazowski meme</h1>
            <p class="blogDate"><i>posted on</i> Sep 7th 2014</p>
            <p class="blogDesc">
              The Mike Wazowski meme features the character Mike Wazowski from the animated film "Monsters, Inc." with his distinctive one-eyed face and humorous expressions. The meme often uses his image to illustrate moments of awkwardness, surprise, or miscommunication, leveraging his expressive and recognizable look. Its popularity stems from the character's relatability and the humor found in his exaggerated reactions.
            </p>
          </div>

        </div>

        <!-- PAGES -->
        <button @click="togglePage('blog')">2</button>
        <button @click="togglePage('blogTwo')">1</button>
        
      </div>
      <div class="homeAds">
        
        <img src="https://pbs.twimg.com/media/E4ALldyVIAc2my1.jpg:large" alt="advertisement">
        <img src="https://i.pinimg.com/originals/7a/7d/1b/7a7d1b122b2ed892ce36b4dc3720b463.jpg" alt="advertisement">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTmGoCQWnO4NDz6L09myAf7y9R13XDNHoiqSg&s" alt="advertisement">

      </div>

    </div>



    <!-- POPULAR -->
    <div class="home" v-if="pageActive.popular">
      <div class="homeContents">
        
        <!--Title-->
        <h1 class="bigFont pageTitle">Popular</h1>

        <!--Blogs-->
        <div class="blogSection">

          <div>
            <img src="https://cache.lahelu.com/image-P0Rv0PSAo-92805" alt="WaduhMeme" class="blogImg" @click="toggleActualBlog('page3')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page3')">Waduh meme</h1>
            <p class="blogDate"><i>posted on</i> Jan 18th 2023</p>
            <p class="blogDesc">
              The "Waduh" meme originates from a viral video of a person named Wicaksono, who in a 2017 Indonesian video, exclaims "Waduh" with a mix of surprise and frustration when encountering a minor inconvenience. The clip, with its expressive reaction and distinctive use of the word "waduh," quickly gained traction online, becoming a popular meme format for conveying exaggerated surprise or dismay. Its simple and relatable expression of mild annoyance made it a favorite for various humorous contexts on social media.
            </p>
          </div>

          <div>
            <img src="https://uploads.dailydot.com/2023/10/Shocked-Meme.jpg?auto=compress&fm=pjpg" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page5')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page5')">Shocked black guy meme</h1>
            <p class="blogDate"><i>posted on</i> Aug 20th 2015</p>
            <p class="blogDesc">
              The Shocked Black Guy meme features a still image of a man named Tariq Nasheed from a 2009 YouTube video, where he displays a wide-eyed, shocked expression. The image gained popularity as a reaction meme to convey surprise, disbelief, or shock in response to unexpected or dramatic statements. Its exaggerated expression and context made it a widely recognizable and versatile meme on social media.
            </p>
          </div>

          <div>
            <img src="https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2019/11/01-Confused-Nick-Young-Meme.png" alt="BlinkingMeme" class="blogImg" @click="toggleActualBlog('page8')">
            <h1 class="bigFont blogName" @click="toggleActualBlog('page8')">Confused meme</h1>
            <p class="blogDate"><i>posted on</i> Feb 18th 2033</p>
            <p class="blogDesc">
              The Confused meme features an image of a man with a perplexed expression, often used to represent confusion or disorientation. The meme typically shows the man in a state of bewilderment, making it a popular choice for illustrating moments when something doesn’t quite make sense. Its humorous portrayal of confusion resonates with many, making it a widely shared and adaptable meme format.
            </p>
          </div>

        </div>
      </div>
      <div class="homeAds">
          
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTsrL6bPFH1qTKHnXOb1Qsg7PahsBvETvWsQA&s" alt="advertisement">
        <img src="https://i.pinimg.com/736x/ba/38/62/ba38623a29eeb78a5e9be6d5cdf7599d.jpg" alt="advertisement">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRlhsMefw6PUT3bpNuu-I9RTa0WD-yPrxeaMQ&s" alt="advertisement">

      </div>
    </div>



    <!-- WEATHER -->
    <div class="weather" v-if="pageActive.weather">
          
      <form @submit.prevent="fetchWeather" class="weatherForm">
        <input v-model="city" type="text" class="cityInput" placeholder="Enter city">
        <button type="submit">Get Weather</button>
      </form>
      <div v-if="weatherData" class="card">
          <h1 class="cityDisplay">{{ weatherData.name }}</h1>
          <p class="tempDisplay">{{ formatTemperature(weatherData.main.temp) }}°F</p>
          <p class="humidityDisplay">Humidity: {{ weatherData.main.humidity }}%</p>
          <p class="descDisplay">{{ weatherData.weather[0].description }}</p>
          <p class="weatherEmoji">{{ getWeatherEmoji(weatherData.weather[0].id) }}</p>
      </div>
      <p v-if="error" class="errorDisplay">{{ error }}</p>

    </div>



    <!-- BLOG PAGE -->
    <div>

      <div class="home" v-if="pageActive.blogPage.page1 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://e3.365dm.com/19/09/2048x1152/skynews-drew-scanlon-blinking-white-guy_4786055.jpg" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">White guy blinking meme</h1>
            <p class="blogDate"><i>posted on</i> Dec 28th 2023</p>
            <p class="blogDesc">
              &emsp;The White Guy Blinking meme traces its origins back to a 2013 live stream on the gaming website Giant Bomb, where video producer Drew Scanlon was part of the show. During the stream, one of his colleagues, Jeff Gerstmann, made a lighthearted and somewhat unexpected comment about "farming with my hoe." Drew, caught off guard by the remark, reacted with a surprised and bemused blink, which was subtly captured on camera. While the moment was minor and went largely unnoticed at the time, it would later gain unexpected fame.<br><br>

              &emsp;Fast forward to 2017, and the internet unearthed this brief clip from the Giant Bomb archives. The blink, with its perfect timing and relatable expression of mild disbelief, resonated with many online users. It quickly spread across social media platforms, becoming a versatile reaction meme. People began using the blinking image or GIF in response to posts or comments that left them surprised, confused, or incredulous, making it a go-to reaction for a wide variety of situations.<br><br>

              &emsp;What made the White Guy Blinking meme so effective was its simplicity and universality. The expression conveyed a mix of confusion, surprise, and mild skepticism that could be applied to countless scenarios. Whether responding to absurd statements, unexpected twists, or just moments of misunderstanding, the meme found a home in numerous online conversations. Its non-verbal nature allowed it to transcend language barriers, making it a globally recognized symbol of a specific, relatable emotion.<br><br>

              &emsp;As the meme gained traction, it evolved into various formats, including still images, GIFs, and even videos, each tailored to different contexts and platforms. The meme's adaptability kept it relevant and widely used across different communities and discussions. It became a staple on Twitter, Reddit, and other social media sites, where users appreciated its ability to succinctly convey a specific reaction that words alone might struggle to express.<br><br>

              &emsp;Despite its origins as a small, fleeting moment on a niche gaming site, the White Guy Blinking meme has endured as a cultural touchstone in the digital age. Drew Scanlon himself acknowledged the meme’s popularity with humor and grace, even using it to raise awareness for charitable causes. The meme stands as a testament to how the internet can take the most unexpected moments and turn them into symbols of shared human experience.<br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://dropshipaja.com/blog/wp-content/uploads/2023/08/contoh-iklan-susu-milo.jpg" alt="advertisement">
          <img src="https://tpc.googlesyndication.com/simgad/17430687534536487893" alt="advertisement">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSXzd7TCMT-ZrQojI2IGRrEHd9Kn_symsTK6A&s" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page2 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://i.insider.com/601448566dfbe10018e00c5d?width=700" alt="Stonks" class="blogPageImg">
            <h1 class="bigFont blogPageName">Stonks meme</h1>
            <p class="blogDate"><i>posted on</i> Dec 23rd 2013</p>
            <p class="blogDesc">
              &emsp;The Stonks meme first appeared in 2017, created by the surrealist meme page Special Meme Fresh on Facebook. The image features a 3D character known as "Meme Man," who is standing in front of a rising stock market graph with the word "stonks" written in bold letters instead of "stocks." This intentional misspelling, combined with the generic and poorly rendered nature of Meme Man, gave the image an absurd, almost nonsensical quality. The meme was quickly picked up by internet users who found its simplicity and surrealism amusing.<br><br>

            &emsp;The meme became popular because it humorously captures the essence of financial ignorance or poor decision-making. Users began sharing it widely to comment on situations where someone makes a questionable investment or a financial decision that seems obviously flawed. The stark contrast between the serious nature of stock markets and the absurdity of the image added to its comedic value. As a result, "Stonks" became a shorthand for mocking or highlighting misunderstandings in the world of economics and investing.<br><br>

            &emsp;What truly propelled the Stonks meme into mainstream internet culture was its adaptability. The basic format of the meme could be easily modified to fit different contexts, whether commenting on personal finance, business decisions, or even broader social issues. Variations of the meme started to appear, with users altering the graph, the character, or the caption to suit their specific message. This flexibility allowed the meme to remain relevant and continually evolve with the times.<br><br>

            &emsp;As the Stonks meme spread, it started to influence conversations beyond just online humor. People began using it in discussions about real-world financial topics, often in a tongue-in-cheek manner. It also found its way into various forms of media and pop culture, being referenced in everything from YouTube videos to Twitter threads. The meme's ability to distill complex ideas into a single, easily recognizable image helped it maintain its popularity across different platforms and audiences.<br><br>

            &emsp;Despite its origins as a simple and absurd joke, the Stonks meme has become an enduring part of internet culture. Its continued relevance can be attributed to its versatility and the way it resonates with the growing interest in finance, especially among younger generations who engage with stocks, cryptocurrency, and other investments online. The meme's evolution and widespread use illustrate how even the most surreal and humorous content can influence and reflect broader societal trends.<br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://i.pinimg.com/originals/a8/21/7d/a8217d88ccb5c481a524af337e2608a3.jpg" alt="advertisement">
          <img src="https://cdnwpseller.gramedia.net/wp-content/uploads/2022/05/07090012/iklan-chitato.webp" alt="advertisement">
          <img src="https://lh3.googleusercontent.com/luCnUYAD4GnzgqCvF99ItNtPmVHm3oE3vq0c0mbAmuGcQ2Zp0bbkYkBi8vpGiRo2ntQ4Fm-7GcT2FcBF0Suu-iGxq51PLOlXpfOj3jTBUm2v9coRxeGKZNzw83mk9V_CJYOSio17bXIbWUDmNBzhvz4" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page3 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://cdn1-production-images-kly.akamaized.net/wizlXmBAHhmiy_OONOjOEExmiEU=/500x500/smart/filters:quality(75):strip_icc():format(webp)/kly-media-production/medias/4473096/original/079167400_1687227614-6682d4172ec12c5a0e8ad5271c3495ee.jpg" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">Waduh meme</h1>
            <p class="blogDate"><i>posted on</i> Jan 18th 2023</p>
            <p class="blogDesc">
              &emsp;The "Waduh" meme first gained popularity from a viral video featuring Wicaksono, an Indonesian individual, who exclaims "Waduh" in a moment of mild frustration or surprise. The video, which was uploaded in 2017, captures his distinctive reaction to an unexpected situation, making it both amusing and relatable. The simplicity of the expression, combined with Wicaksono's animated delivery, quickly resonated with viewers. <br><br>

              &emsp;The term "Waduh" itself is an Indonesian expression that conveys a sense of surprise or annoyance, and in the video, it is used in a context that amplifies the comedic effect. As the video spread across social media platforms, the clip was shared and remixed in various formats, turning it into a widely recognized meme. The meme became popular for its ability to succinctly express a range of minor frustrations or unexpected events. <br><br>

              &emsp;The meme's appeal lies in its universality; while "Waduh" is specific to Indonesian culture, the emotional reaction it conveys is universally understood. Internet users from different backgrounds began using the meme to comment on everyday annoyances or surprising moments, adapting the expression to fit a variety of humorous contexts. The meme's flexibility allowed it to be used in numerous scenarios, making it a versatile addition to online humor. <br><br>

              &emsp;As the "Waduh" meme continued to gain traction, it also started influencing other forms of media and pop culture. It was featured in various online discussions, parody videos, and even in some traditional media, demonstrating its wide-reaching impact. The meme's use of exaggerated expression and relatable content helped it maintain relevance across different digital spaces and audience demographics. <br><br>

              &emsp;Despite its origins as a simple reaction video, the "Waduh" meme has evolved into a significant cultural touchstone within internet culture. Its continued popularity reflects how a small, relatable moment can resonate widely and become a lasting symbol of common human experiences. The meme's success highlights the power of digital content to transform ordinary reactions into global phenomena. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://lh4.googleusercontent.com/9ibWLmWmYaG6spJtvFK8jBbJtMXoP2Bq721cOt27woj1zv6Ov7wA5orcbqAVPIa-60c-JEHYvVCqyZYlXRDhz_UA14kHsmMARlro_vju3kzqh9s8VZWb_cg3Fec__9yJG9P8Vze5dmTelyYclZ_Bt1A" alt="advertisement">
          <img src="https://imgx.sonora.id/crop/0x0:0x0/x/photo/2023/05/18/whatsapp-image-2022-11-13-at-16-20230518124718.jpeg" alt="advertisement">
          <img src="https://evermos.com/home/wp-content/uploads/2023/11/contoh-iklan-produk-perawatan-wajah.webp" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page4 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://upload.wikimedia.org/wikipedia/en/f/ff/SuccessKid.jpg" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">Success kid meme</h1>
            <p class="blogDate"><i>posted on</i> Jun 10th 2022</p>
            <p class="blogDesc">
              &emsp;The Success Kid meme originated from a 2007 photograph of a young boy named Sammy Griner, taken by his mother during a day at the beach. In the image, Sammy is seen with a determined expression, his fist clenched triumphantly, as if celebrating a small victory. This candid moment captured by his mother would later become a symbol of personal achievement and success. <br><br>

              &emsp;The photo's journey to internet fame began when it was shared online and quickly resonated with many users who saw it as an emblem of triumph and perseverance. The image's simplicity and Sammy's expressive pose made it ideal for pairing with a variety of captions that highlighted everyday victories and humorous situations. This versatility allowed the meme to spread rapidly across social media platforms. <br><br>

              &emsp;The Success Kid meme's appeal lies in its universal representation of overcoming challenges or achieving goals, no matter how small. The meme became widely used to celebrate personal achievements, from completing tasks to achieving minor successes, often framed in a humorous or exaggerated manner. Its relatability and positive connotation contributed to its enduring popularity. <br><br>

              &emsp;As the meme continued to gain traction, it evolved beyond just an image of success to become a significant part of internet culture. It was featured in various contexts, including marketing campaigns, social media posts, and even merchandise. The Success Kid's image was used to convey messages of inspiration and motivation, reflecting its widespread influence. <br><br>

              &emsp;Despite its origins as a simple photograph, the Success Kid meme has become a lasting symbol of achievement and perseverance in the digital age. Sammy Griner's image represents how a single, relatable moment can capture the imagination of millions and become a powerful tool for expressing joy and success online. The meme's enduring presence highlights the impact that everyday moments can have in shaping internet culture. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://storage.googleapis.com/fastwork-static/7d8c897d-4955-4ca8-8453-0010edaba793.jpg" alt="advertisement">
          <img src="https://blog.sribu.com/wp-content/uploads/2023/12/b79a9d4c-c21d-4df0-b3af-a0d3f1c5ed80.jpg" alt="advertisement">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbwqWgTO2ax1zw-PEjUsLqLKOFJb8Jft7D4g&s" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page5 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://uploads.dailydot.com/2023/10/Shocked-Meme.jpg?auto=compress&fm=pjpg" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">Shocked black guy meme</h1>
            <p class="blogDate"><i>posted on</i> Aug 20th 2015</p>
            <p class="blogDesc">
              &emsp;The Shocked Black Guy meme originates from a 2009 YouTube video featuring Tariq Nasheed, who is captured in a moment of intense surprise. In the video, Tariq reacts with a wide-eyed, open-mouthed expression that perfectly conveys shock and disbelief. This particular frame from the video became iconic due to its powerful visual impact and relatable reaction to unexpected or dramatic news. <br><br>

              &emsp;The image quickly gained traction on social media, where it was adopted as a reaction meme for various scenarios. Internet users began pairing the shocked expression with captions that highlighted their own moments of surprise or incredulity. The meme’s ability to convey a strong emotional reaction with just a single image contributed to its rapid spread and widespread use. <br><br>

              &emsp;What made the Shocked Black Guy meme particularly effective was its versatility. The exaggerated nature of Tariq Nasheed’s expression allowed it to be applied to a broad range of contexts, from humorous situations to more serious surprises. This adaptability made it a popular choice for users looking to express their reactions to unexpected statements or events. <br><br>

              &emsp;As the meme continued to circulate, it became a staple in various online discussions and media. Its presence was felt across platforms like Twitter, Reddit, and Facebook, where it was used to emphasize or parody shocking or surprising content. The meme's widespread recognition and application highlighted its significant role in internet culture and meme history. <br><br>

              &emsp;Despite its origins in a single YouTube video, the Shocked Black Guy meme has endured as a prominent example of how a simple, expressive image can become a powerful tool for communication online. Tariq Nasheed’s expressive reaction captured a universal feeling of surprise, demonstrating how viral content can resonate with people across different contexts and platforms. The meme remains a testament to the impact of visual expression in digital culture. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://ik.imagekit.io/tvlk/blog/2022/10/Socmed_All-Guest-Star_21-Okt-1-577x1024.jpg?tr=dpr-2,w-675" alt="advertisement">
          <img src="https://www.jogjapromo.com/wp-content/uploads/2020/08/voucher-code-reddoorz-2020-576x1024.jpeg" alt="advertisement">
          <img src="https://mik.fkt.ugm.ac.id/wp-content/uploads/sites/1107/2022/03/Poster-Maba-Semester-Gasal-TA-2022-2023-scaled.jpg" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page6 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://i.kym-cdn.com/entries/icons/facebook/000/027/475/Screen_Shot_2018-10-25_at_11.02.15_AM.jpg" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">Surprised pikachu meme</h1>
            <p class="blogDate"><i>posted on</i> Feb 13th 2008</p>
            <p class="blogDesc">
              &emsp;The Surprised Pikachu meme comes from a scene in the Pokémon animated series where Pikachu, the beloved yellow Pokémon, shows a look of shock and surprise. This particular reaction shot captures Pikachu with wide eyes and a surprised mouth, making it a memorable and expressive image. The scene originally aired in an episode where Pikachu reacts to unexpected news, but its impact extended far beyond the show. <br><br>

              &emsp;The meme gained traction on the internet as users began to pair the surprised Pikachu image with captions that humorously depict moments of shock or disbelief. It became a popular way to illustrate scenarios where someone is caught off guard by outcomes that were actually foreseeable or expected. The contrast between the predictable nature of the events and Pikachu's exaggerated reaction adds to the comedic effect. <br><br>

              &emsp;The Surprised Pikachu meme's appeal lies in its simplicity and versatility. The image's expressive nature allows it to be used in a wide range of contexts, from everyday surprises to more specific scenarios. Its adaptability has made it a staple in online discussions and meme culture, where it continues to be used to emphasize moments of unexpected realization. <br><br>

              &emsp;As the meme spread across various social media platforms, it became a well-known symbol of humorous disbelief. Its presence was felt on platforms like Twitter, Reddit, and Facebook, where users creatively applied the image to diverse situations. The meme's popularity highlights how a single, iconic reaction can resonate with a broad audience and become a lasting part of internet culture. <br><br>

              &emsp;Despite its origins in a simple animated scene, the Surprised Pikachu meme has become an enduring example of how visual expressions can capture universal feelings of surprise. Pikachu's shocked face effectively conveys a sense of disbelief that many find relatable, demonstrating the power of meme culture to transform a moment from a TV show into a widely recognized internet phenomenon. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://i.pinimg.com/736x/51/a3/f8/51a3f8ed21e0923e9de72998f5d92a18.jpg">
          <img src="https://i.pinimg.com/736x/c9/45/48/c94548f8f968dcfbd5a1ee6d18fcb8d4.jpg">
          <img src="https://i.pinimg.com/736x/59/cd/b3/59cdb3df163b2f7df34e7638bf4e5bcf.jpg" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page7 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://us-tuna-sounds-images.voicemod.net/e54c6d53-6c5d-47e3-9feb-6dc0d22437e1-1702824730148.jpg" alt="Stonks" class="blogPageImg">
            <h1 class="bigFont blogPageName">The rock eyebrow meme</h1>
            <p class="blogDate"><i>posted on</i> Apr 3rd 2013</p>
            <p class="blogDesc">
              &emsp;The Rock Eyebrow meme centers around a memorable image of Dwayne "The Rock" Johnson, captured mid-expression with one eyebrow raised. This distinctive pose is one of Johnson's signature looks, showcasing his ability to convey a range of emotions with just a single eyebrow movement. The image originates from his appearances in various films and public appearances, where his charismatic and expressive demeanor made a lasting impression. <br><br>

              &emsp;The meme began to gain traction as internet users started to repurpose the eyebrow-raising image to express skepticism, curiosity, or surprise in a humorous way. The Rock's iconic eyebrow lift, combined with the versatility of the image, made it a popular choice for various captions and contexts. The meme’s ability to succinctly convey a reaction while adding a touch of humor contributed to its widespread use. <br><br>

              &emsp;What makes the Rock Eyebrow meme particularly effective is its adaptability. Users have creatively employed the image to comment on situations ranging from minor surprises to more complex scenarios involving disbelief or questioning. The meme's flexibility allows it to fit a broad range of contexts, making it a favorite for conveying a range of reactions online. <br><br>

              &emsp;As the meme continued to spread across social media platforms, it solidified its place in internet culture. It was used in various formats, including tweets, memes, and even merchandise, further cementing The Rock’s iconic expression in the digital landscape. The meme’s popularity underscores how a single, recognizable image can become a significant part of online discourse. <br><br>

              &emsp;Despite its roots in entertainment media, the Rock Eyebrow meme has transcended its original context to become a universal symbol of reaction and emotion. The Rock’s expressive eyebrow lift captures a moment of genuine curiosity or skepticism, demonstrating how powerful a single facial expression can be in digital culture. The meme remains a testament to the impact of charismatic and memorable visuals in shaping internet humor. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://i.pinimg.com/236x/ce/fb/7e/cefb7ef2600ac6e6a035addd1b2b6e54.jpg">
          <img src="https://i.pinimg.com/originals/32/25/27/32252757b7f59d7df3875db8db80a655.jpg">
          <img src="https://lh3.googleusercontent.com/luCnUYAD4GnzgqCvF99ItNtPmVHm3oE3vq0c0mbAmuGcQ2Zp0bbkYkBi8vpGiRo2ntQ4Fm-7GcT2FcBF0Suu-iGxq51PLOlXpfOj3jTBUm2v9coRxeGKZNzw83mk9V_CJYOSio17bXIbWUDmNBzhvz4" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page8 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2019/11/01-Confused-Nick-Young-Meme.png" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">Confused meme</h1>
            <p class="blogDate"><i>posted on</i> Feb 18th 2033</p>
            <p class="blogDesc">
              &emsp;The Confused meme is centered around an image of a man who appears visibly puzzled and disoriented. This particular expression, characterized by wide eyes and a furrowed brow, effectively captures the essence of confusion. The image has become a popular visual representation of moments where something is unclear or perplexing. <br><br>

              &emsp;The meme's appeal lies in its ability to convey a strong sense of bewilderment with a simple, yet expressive image. Internet users have widely adopted the meme to humorously depict situations where logic or context seems lacking. The man’s confused look serves as a relatable reaction to scenarios that defy understanding or common sense. <br><br>

              &emsp;In its various iterations, the Confused meme is often paired with captions that highlight the absurdity or complexity of a situation. These captions typically play off the man’s puzzled expression, adding a layer of humor to the image. This combination of visual and textual elements allows the meme to address a wide range of confusing or baffling topics. <br><br>

              &emsp;As the meme gained popularity, it spread across different social media platforms, becoming a staple in online conversations. It has been used to comment on everything from confusing news stories to quirky everyday occurrences. The meme’s versatility and relatable depiction of confusion have made it a go-to choice for illustrating moments of perplexity. <br><br>

              &emsp;The Confused meme’s enduring success underscores the power of visual expressions in digital communication. Its simple yet effective portrayal of confusion resonates with many, demonstrating how a single image can capture a universal experience. The meme remains a prominent example of how relatable content can become a significant part of internet culture. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://bithourproduction.com/blog/wp-content/uploads/2023/03/a235886a7cbb30fc5216c2e3d82e1601.png" alt="advertisement">
          <img src="https://awsimages.detik.net.id/community/media/visual/2016/06/06/c5e6d90d-612d-4769-a7f3-907584691238_34.jpg?w=600&q=90" alt="advertisement">
          <img src="https://awsimages.detik.net.id/community/media/visual/2024/06/06/inside-out-2_34.jpeg?w=650" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page9 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://pbs.twimg.com/media/FrmIRCcagAIdvhW.jpg" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">Biar apa? biarin meme</h1>
            <p class="blogDate"><i>posted on</i> Aug 17th 1945</p>
            <p class="blogDesc">
              &emsp;The "Biar apa? Biarin" meme originates from a viral Indonesian video featuring a man who responds with a casual "Biar apa? Biarin," which translates to "Why? Just let it be." In the video, the man’s nonchalant demeanor and relaxed attitude toward a question or problem capture a humorous and carefree approach to handling situations. The phrase exemplifies a laid-back philosophy, making it both memorable and relatable. <br><br>

              &emsp;The meme gained traction as internet users began to adopt the phrase to humorously depict moments when they choose to ignore or not worry about problems. The image of the man, combined with his indifferent response, became a symbol of a relaxed and easygoing attitude toward life's challenges. This approach resonated with many, who found the nonchalant response to be a refreshing take on dealing with issues. <br><br>

              &emsp;In various iterations of the meme, the "Biar apa? Biarin" phrase is often paired with captions that emphasize a lack of concern or the decision to let things unfold without interference. The meme’s appeal lies in its ability to humorously address situations where people might otherwise feel pressured to act. The combination of the man’s expression and the phrase adds a layer of lightheartedness to the message. <br><br>

              &emsp;As the meme continued to spread across social media platforms, it became a popular way to express a carefree attitude. It was used to comment on everything from minor inconveniences to more significant life decisions, reflecting the meme’s versatility and broad appeal. The "Biar apa? Biarin" meme’s widespread use underscores its resonance with audiences who appreciate its humor and relaxed perspective. <br><br>

              &emsp;The success of the "Biar apa? Biarin" meme highlights how a simple phrase and expressive video can capture a universal sentiment. Its ability to convey a humorous and indifferent attitude towards problems has made it a notable part of internet culture. The meme remains a testament to how relatable and laid-back expressions can connect with a wide audience and become enduring elements of digital humor. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://radiopinguinfm.com/images/news/md/2024613154344.jpg" alt="advertisement">
          <img src="https://blog.sribu.com/wp-content/uploads/2023/12/b79a9d4c-c21d-4df0-b3af-a0d3f1c5ed80.jpg" alt="advertisement">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbwqWgTO2ax1zw-PEjUsLqLKOFJb8Jft7D4g&s" alt="advertisement">

        </div>
      </div>

      <div class="home" v-if="pageActive.blogPage.page10 === true">
        <div class="homeContents">

          <!--Blogs-->
          <div class="blogSection">

            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQv7YsjKKlyiMikvRYW8fxYuXLVO8jEM3X45Q&s" alt="WhiteGuyBlinking" class="blogPageImg">
            <h1 class="bigFont blogPageName">Mike Wazowski meme</h1>
            <p class="blogDate"><i>posted on</i> Sep 7th 2014</p>
            <p class="blogDesc">
              &emsp;The Mike Wazowski meme originates from the animated film "Monsters, Inc.," produced by Pixar Animation Studios and released in 2001. Mike Wazowski, a green, one-eyed monster voiced by Billy Crystal, is one of the film's main characters known for his humorous and expressive personality. His distinctive appearance and exaggerated facial expressions made him a memorable and relatable character, providing fertile ground for meme creation. <br><br>

              &emsp;The meme gained popularity due to Mike Wazowski's versatile expressions, which can convey a wide range of emotions, from surprise to awkwardness. Users began to repurpose his character’s image, often pairing it with captions that highlight humorous or relatable situations. The meme's ability to capture the essence of various social interactions with a single, recognizable image contributed to its widespread appeal. <br><br>

              &emsp;One of the most common uses of the Mike Wazowski meme is to depict moments of social discomfort or unexpected surprises. For instance, his wide-eyed, surprised expression is often used to illustrate situations where someone is caught off guard or experiences an awkward encounter. This application of the meme resonates with many, who find humor in the character's exaggerated reactions to relatable scenarios. <br><br>

              &emsp;As the meme continued to evolve, it became a popular fixture on social media platforms such as Twitter, Reddit, and Facebook. The versatility of Mike Wazowski’s expressions allowed the meme to adapt to various contexts and trends, further solidifying its place in internet culture. Its enduring popularity highlights how a single character's expressive features can become a powerful tool for conveying humor online. <br><br>

              &emsp;The Mike Wazowski meme exemplifies how animated characters can transcend their original media to become significant parts of internet humor. The character’s distinctive look and ability to express a wide range of emotions have made him a favorite in meme culture. The continued use and adaptation of Mike Wazowski’s image demonstrate the lasting impact of memorable film characters on digital communication and humor. <br><br>
            </p>

          </div>

        </div>
        <div class="homeAds">
          
          <img src="https://ik.imagekit.io/tvlk/blog/2022/10/Socmed_All-Guest-Star_21-Okt-1-577x1024.jpg?tr=dpr-2,w-675" alt="advertisement">
          <img src="https://www.jogjapromo.com/wp-content/uploads/2020/08/voucher-code-reddoorz-2020-576x1024.jpeg" alt="advertisement">
          <img src="https://upload.wikimedia.org/wikipedia/id/6/6d/Frozen_II_%282019_poster%29.jpg" alt="advertisement">

        </div>
      </div>

    </div>



    <!-- FOOTER -->
    <footer>
      <p class="bigFont">© 2024 MemeHistory | Privacy policy</p>
    </footer>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  data() {
    return {

      pageActive: {

        blog: true,
        blogTwo: false,
        popular: false,
        weather: false,

        blogPage: {
          page1: false,
          page2: false,
          page3: false,
          page4: false,
          page5: false,
          page6: false,
          page7: false,
          page8: false,
          page9: false,
          page10: false,

          page11: false,
          page12: false,
          page13: false,
        }

      },



      blogPreview: {

      },



      city: '',
      weatherData: null,
      error: null


    }
  },

  methods: {
    togglePage(target) {
      this.pageActive.blog = false
      this.pageActive.popular = false
      this.pageActive.weather = false

      for (let i = 1; i < 14; i++) {
        let value = `page${i}`
        this.pageActive.blogPage[value] = false
      }

      if (target === 'blog') {
        this.pageActive.blog = true
        this.pageActive.blogTwo = false
        this.pageActive.popular = false
        this.pageActive.weather = false
      } else if (target === 'popular') {
        this.pageActive.blog = false
        this.pageActive.blogTwo = false
        this.pageActive.popular = true
        this.pageActive.weather = false
      } else if (target === 'blogTwo') {
        this.pageActive.blog = false
        this.pageActive.blogTwo = true
        this.pageActive.popular = false
        this.pageActive.weather = false
      } else if (target === 'weather') {
        this.pageActive.blog = false
        this.pageActive.blogTwo = false
        this.pageActive.popular = false
        this.pageActive.weather = true
      }
    },

    toggleActualBlog(target) {
      this.pageActive.blog = false
      this.pageActive.blogTwo = false
      this.pageActive.popular = false

      this.pageActive.blogPage[target] = true
    },

    getAdImg() {
      let num = Math.round(Math.random() * (1 - 10) + 1)
    },





    async fetchWeather() {
      const apiKey = "32590574af4fcd6726fa269cfb6cc029";
      this.error = null;
      if (this.city) {
          try {
              const weatherData = await this.getWeatherData(this.city, apiKey);
              this.weatherData = weatherData;
          } catch (error) {
            document.querySelector('.card').style.display="none";
              this.error = "Could not fetch weather data";
              console.error(error);
          }
      } else {
          this.error = "Please enter a city";
      }
    },
    async getWeatherData(city, apiKey) {
        const apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}`;
        const response = await fetch(apiUrl);
        if (!response.ok) {
            throw new Error("Could not fetch weather data");
        }
        return await response.json();
    },
    getWeatherEmoji(weatherId) {
        switch (true) {
            case (weatherId >= 200 && weatherId < 300):
                return "🌩️"; // Thunderstorm
            case (weatherId >= 300 && weatherId < 400):
                return "🌦️"; // Drizzle
            case (weatherId >= 500 && weatherId < 600):
                return "🌧️"; // Rain
            case (weatherId >= 600 && weatherId < 700):
                return "❄️"; // Snow
            case (weatherId >= 700 && weatherId < 800):
                return "🌫️"; // Atmosphere
            case (weatherId === 800):
                return "☀️"; // Clear sky
            case (weatherId >= 801 && weatherId < 810):
                return "🌤️"; // Clouds
            default:
                return "🌈"; // Default or unknown
        }
    },
    formatTemperature(temp) {
        return ((temp - 273.15) * 9/5 + 32).toFixed(1);
    }
  }
}
</script>

<style>
/* GENERAL */
* {
  margin: 0px;
  padding: 0px;
  font-family: "Open Sans", system-ui;
}
*::selection {
  background-color: rgb(255, 255, 0, 0.8);
  color: rgba(0, 0, 0, 0.8);
}

/*  font-family: "Baskervville SC", serif; */
/* font-family: "Open Sans", system-ui; */
.bigFont {
  font-family: "Baskervville SC", serif;
}
.smallFont {
  font-family: "Open Sans", system-ui; 
}





/*  HEADER */
nav {
  height: 80px;
  background-color: crimson;
  display: flex;
  color: white;
  align-items: center;
  padding: 0px 50px;
}
nav :first-child {
  flex: 1;
  font-size: 30px;
  font-weight: 600;
}
nav :last-child, nav :nth-child(3) {
  margin-left: 50px;
}
nav :nth-child(2), nav :nth-child(3), nav :last-child {
  cursor: pointer;
}





/*  HOME */
.home {
  display: flex;
  background-color: rgb(245, 245, 245);
  padding: 75px 100px 100px 100px;
}
.homeContents {
  flex: 1;
  margin-right: 50px;
}
.homeAds {
  width: 200px;
}
.home h1 {
  font-size: 50px;
}
.pageTitle {
  margin-bottom: 50px;
  border-bottom: 2px solid black;
}
.blogImg {
  width: 100%;
  height: 300px;
  object-fit: cover;
  cursor: pointer;
}
.blogImg:hover {
  box-shadow: 10px, 10px, 10px, rgba(0, 0, 0, 0.8);
}
.blogName {
  cursor: pointer;
}
.blogDate {
  margin: 30px 0px;
  font-size: 14px;
  color: rgb(182, 0, 0);
}
.blogDesc {
  font-size: 18px;
  margin-bottom: 200px;
}
.blogSection {
  margin-bottom: 150px;
}

.homeAds img {
  width: 100%;
  margin-bottom: 100px;
  cursor: pointer;
}

.home button {
  border: none;
  background-color: rgba(0, 0, 0, 0);
  color: crimson;
  font-size: large;
  text-decoration: underline;
  width: 25px;
  height: 30px;
  margin: 10px;
  cursor: pointer;
}
.home button:hover {
  background-color: crimson;
  color: white;
  border: none;
}




/*  BLOG PAGE */
.blogPageImg {
  width: 100%;
}
.blogPageName {
  cursor: default;
  border-bottom: 2px solid black;
}




/*  FOOTER */
footer {
  height: 50px;
  background-color: gray;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-size: small;
}





/* WEATHER */
.weather {
  display: flex;
  flex-direction: column;
  background-color: rgb(245, 245, 245);
  padding: 75px 100px 100px 100px;
  height: 100vh;
  align-items: center;
}
.weatherForm {
  margin-bottom: 20px;
}
.cityInput {
  padding: 10px;
  border: none;
  margin-right: 20px;
  border-radius: 5px;
}
.weatherForm button {
  border-radius: 5px;
  background-color: green;
  color: white;
  padding: 10px;
  border: none;
  cursor: pointer;
}
.card {
  width: 266px;
  height: 400px;
  padding: 10px;
  background-color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  border-radius: 5px;
}
.cityDisplay, .tempDisplay {
  font-size: 40px;
  margin-bottom:  10px;
}
.card {
  font-size: 20px;
}
.card p {
  margin: 5px;
}
.weatherEmoji {
  font-size: 70px;
}
</style>