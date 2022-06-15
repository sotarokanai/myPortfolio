<template>
    <div class="works">
        <div class="content-area">
            <ttlTxt>デッサンと学校基礎課題＜一部＞</ttlTxt>
            <paragraph>静物デッサンとイメージデッサン、学校（桑沢デザイン研究所）基礎課題の一部と入学試験時の課題制作であるポスターの紹介。<br>＜順次更新予定＞</paragraph>
            <ttlTxt>デッサン</ttlTxt>
            <contentImage
            :src="require(`~/assets/img/other/IMG_2178.jpg`)"        
            ></contentImage>
            <paragraph>2020年制作</paragraph>
             <contentImage
            :src="require(`~/assets/img/other/IMG_2181.jpg`)"        
            ></contentImage>
            <paragraph>2021年制作</paragraph>
             <contentImage
             default_size="700px"
            :src="require(`~/assets/img/other/IMG_2182.jpg`)"        
            ></contentImage>
            <paragraph>2021年制作</paragraph>
             <ttlTxt>イメージデッサン</ttlTxt>
              <contentImage
              default_size="700px"
            　:src="require(`~/assets/img/other/IMG_2179.jpg`)"        
            ></contentImage>
            <paragraph>2021年制作<br>紙コップをモチーフに用意し、そこからイメージデッサンを行った。紙コップを「蛸壺」にみたて、太い脚を持つタコが、紙コップを突き破るシーンを描写し、タコの力強さを表現した。</paragraph>
             <contentImage
              default_size="700px"
            　:src="require(`~/assets/img/other/IMG_2184.jpg`)"        
            ></contentImage>
            <paragraph>2021年制作<br>マカロンケースをモチーフに用意し、そこからイメージデッサンを行った。透明のカーバーケースの中へマカロンケースがロープを引きちぎりながら侵入してくる<br>シーンを描写し、マカロンの「かわいらしさ」から離れた「緊迫感」や「閉鎖感」を表現した。</paragraph>
             <ttlTxt>桑沢デザイン研究所入学試験課題「自分の個展をイメージしたポスター制作」</ttlTxt>
              <contentImage
              default_size="700px"
            　:src="require(`~/assets/img/other/poster_fin.jpg`)"        
            ></contentImage>
             <paragraph>2021年制作<br>＜コメント＞<br>　「ランダム性」「偶然性」「プログラム」この3つが今回の展覧会のキーワードだ。
                私たちは日常の中でランダム性や偶然性に深く影響されている。神社でおみくじを引いた時、私たちはそのランダムな結果により「嬉しさ」や「不安」など様々な感情が生じる。私はこのような人間が知り得ない結果をもたらす「ランダム性」、「偶然性」に面白さを感じ、今回の展覧会を企画した。プログラムによって作り上げられた数値やランダム性により生み出された形状が、偶然私たちの心を揺さぶる造形に変化する。以上を踏まえ「ランダム性」や「偶然性」を視覚的に楽しんでいただけるよう作品を制作した。<br>　ポスター中央のオブジェクトは長方形のメッシュの頂点位置にランダムな値を代入し波打った形状を生成し、そこに不規則な数列を当てはめランダム性を表現した。ランダム性を想起されるオブジェクトとコンピューターから生み出されるアルゴリズミックで無機質なイメージを装飾として組み合わせ展覧会のテーマを表現した。
            </paragraph>
            <ttlTxt>tool</ttlTxt>
            <paragraph>TouchDesiner, Figma</paragraph>
            <ttlTxt>桑沢デザイン研究所　基礎課題</ttlTxt>
            <ttlTxt>グリッドピクトグラム</ttlTxt>
              <contentImage
            　:src="require(`~/assets/img/other/220614_2135_001-3.jpg`)"        
            ></contentImage>
            <paragraph>2021年5月制作<br>縦横10マスのグリッド上のキャンバスに遮光器土偶（右）と仮面の女神（左）をピクトグラム化した。色・高さ・幅を揃えてピクトグラムとしての共通性を重要視した。</paragraph>
             <ttlTxt>色彩表現＜四季の移ろい＞</ttlTxt>
              <contentImage
            　:src="require(`~/assets/img/other/220614_2140_001-3.jpg`)"        
            ></contentImage>
                <paragraph>2021年5月制作</paragraph>
                <ttlTxt>tool</ttlTxt>
                <paragraph>アクリル絵の具<br><br>＜以後、順次公開予定＞</paragraph>
        </div>
    </div>
</template>

<style lang="scss">
.works {
    width: 100%;
    overflow: hidden;
    .content-area {
        padding-top: 38px;
        width: 1144px;
        margin: 0 auto;
        iframe {
            width: 100%;
            height: 400px;
            margin-bottom: 34px;
        }
    }
}

@include mobile {
    .works {
        .content-area {
            width: v(680);
            padding-top: v(38);
            iframe {
            width: v(680);
            margin-bottom: v(34);
            }
        }
    }
}
</style>