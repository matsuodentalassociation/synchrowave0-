<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Synchro Wave 01 - 睡眠改善サポート</title>
    
    <!-- フォント読み込み -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&family=Noto+Sans+JP:wght@400;500;700&display=swap" rel="stylesheet">
    
    <style>
       * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Noto Sans JP', sans-serif;
    line-height: 1.6;
    background-color: white;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* ヘッダーリボン */
.header-ribbon {
    width: 100%;
    height: 400px;
    background-image: url('https://i.imgur.com/YNMOWGB.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    position: relative;
    z-index: 10;
}

/* ヒーローセクション */
.hero {
    background-color: white;
    color: #333;
    text-align: center;
    padding: 80px 0;
    position: relative;
    overflow: hidden;
}

.hero .container {
    position: relative;
    z-index: 2;
}

/* SYNCHRO WAVE 01 スタイル */
.hero-brand {
    font-family: 'Montserrat', 'Arial', sans-serif;
    font-size: 4rem;
    font-weight: 700;
    letter-spacing: 0.05em;
    margin-bottom: 2rem;
    color: #ff6b6b;
    text-transform: uppercase;
    white-space: nowrap;
}

/* メインタイトル */
.hero h1 {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 1.5rem;
    color: #333;
}

/* デスクトップ用テキスト表示 */
.desktop-text {
    display: inline;
}

/* モバイル用テキスト非表示 */
.mobile-text {
    display: none;
}

/* サブタイトル */
.hero-subtitle {
    font-size: 1.3rem;
    font-weight: 400;
    line-height: 1.6;
    margin-bottom: 2.5rem;
    color: #666;
}

/* 問題提起セクション */
.problem-section {
    background-color: white;
    color: #333;
    text-align: center;
    padding: 100px 0;
    position: relative;
    overflow: hidden;
}

.problem-section .container {
    position: relative;
    z-index: 2;
}

/* 問題提起セクションタイトル */
.problem-section h2 {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.5rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 3rem;
    color: #333;
    white-space: nowrap;
}

/* 問題定義用画像 */
.problem-image {
    width: 100%;
    max-width: 800px;
    height: auto;
    margin: 0 auto 3rem;
    display: block;
    border-radius: 15px;
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.1);
}

/* 問題リスト */
.problem-list {
    list-style: none;
    max-width: 900px;
    margin: 0 auto 3rem;
    text-align: left;
    padding-left: 0;
}

.problem-item {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 1.8rem 2rem 1.8rem 4rem;
    margin-bottom: 1.8rem;
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    position: relative;
    transition: all 0.4s ease;
    box-shadow: 0 4px 20px rgba(255, 107, 107, 0.15);
}

.problem-item:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-4px);
    box-shadow: 0 12px 40px rgba(255, 107, 107, 0.25);
    border-color: rgba(255, 107, 107, 0.4);
}

.problem-item::before {
    content: '✓';
    position: absolute;
    left: 1rem;
    top: 50%;
    transform: translateY(-50%);
    width: 2.2rem;
    height: 2.2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    color: white;
    font-size: 1.1rem;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
}

/* CTA テキスト */
.problem-cta {
    font-size: 1.5rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-top: 2.5rem;
}

/* 新しい睡眠サポートセクション */
.solution-section {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.solution-section .container {
    position: relative;
    z-index: 2;
}

.section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

/* PC用タイトル - 改行しないよう調整 */
.section-title-desktop {
    display: inline;
    white-space: nowrap;
}

.section-title-mobile {
    display: none;
}

/* コンテンツ横並びエリア */
.content-flex {
    display: flex;
    align-items: flex-start;
    gap: 3rem;
    margin-bottom: 4rem;
    max-width: 1100px;
    margin-left: auto;
    margin-right: auto;
}

/* 説明テキストカード */
.description-card {
    flex: 1;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    color: #333;
}

.description-card p {
    font-size: 1.3rem;
    font-weight: 500;
    line-height: 1.8;
    margin-bottom: 1.2rem;
    color: #333;
}

.description-card p:last-child {
    margin-bottom: 0;
}

/* 博士画像エリア */
.doctor-image {
    flex: 0 0 300px;
    text-align: center;
}

.doctor-image img {
    width: 100%;
    height: auto;
    border-radius: 15px;
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
    border: 3px solid rgba(255, 107, 107, 0.3);
}

.doctor-caption {
    font-size: 0.9rem;
    color: #666;
    margin-top: 0.5rem;
}

/* シューマン共振発信器画像 - 1.5倍拡大 */
.device-image {
    text-align: center;
    margin-bottom: 4rem;
}

.device-image img {
    max-width: 600px;
    width: 100%;
    height: auto;
    margin: 2rem 0 1rem 0;
    filter: drop-shadow(0 8px 32px rgba(0, 0, 0, 0.2));
    border-radius: 10px;
}

/* デバイス画像キャプション */
.device-caption {
    font-size: 1.1rem;
    color: #666;
    margin-top: 1rem;
    font-weight: 500;
    white-space: nowrap;
}

/* PC用キャプション表示 */
.device-caption-desktop {
    display: inline;
}

/* スマホ用キャプション非表示 */
.device-caption-mobile {
    display: none;
}

/* 特徴カードエリア */
.features-flex {
    display: flex;
    gap: 3rem;
    max-width: 1100px;
    margin: 0 auto;
}

.feature-card {
    flex: 1;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    text-align: center;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.feature-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

.feature-icon {
    font-size: 3rem;
    margin-bottom: 1.5rem;
    display: block;
}

.feature-card h3 {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    color: #333;
}

.feature-card p {
    font-size: 1.1rem;
    font-weight: 500;
    line-height: 1.7;
    color: #333;
}

/* 右側の特徴カード（ベッドサイド）のテキストを左詰めに */
.feature-card.left-align {
    text-align: left;
}

.feature-card.left-align .feature-icon {
    text-align: center;
}

.feature-card.left-align h3 {
    text-align: center;
}

/* ========== セクション4専用CSS（セクション1-3デザインに統一） ========== */

/* 医学的根拠セクション */
.medical-evidence-1 {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.evidence-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
    position: relative;
    z-index: 2;
}

.evidence-main-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 1.5rem;
    text-align: center;
    color: #333;
}

.subsection-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 1.6rem;
    font-weight: 500;
    line-height: 1.5;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

.evidence-cards {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    max-width: 1100px;
    margin: 0 auto;
}

.evidence-card {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.evidence-card:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

.card-header {
    margin-bottom: 2rem;
}

.card-title {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: #333;
    line-height: 1.3;
    text-align: center;
}

.card-subtitle {
    font-size: 1.1rem;
    font-weight: 500;
    line-height: 1.6;
    color: #333;
    text-align: left;
}

.card-content h5 {
    font-size: 1.4rem;
    font-weight: 600;
    margin-bottom: 1.5rem;
    color: #333;
    text-align: center;
}

.evidence-details {
    margin-bottom: 2rem;
}

.evidence-details summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: #333;
    cursor: pointer;
    padding: 1rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    border: 2px solid rgba(255, 107, 107, 0.2);
    transition: all 0.3s ease;
    text-align: center;
}

.evidence-details summary::before {
    content: '▼ ';
    margin-right: 0.5rem;
}

.evidence-details summary:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    border-color: rgba(255, 107, 107, 0.4);
}

.improvement-data {
    padding: 1.5rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    margin-top: 1rem;
    border: 1px solid rgba(255, 107, 107, 0.1);
}

.improvement-data p {
    font-size: 1.1rem;
    line-height: 1.6;
    margin-bottom: 1rem;
    color: #dc2626;
}

.improvement-data ul {
    list-style: none;
    padding: 0;
}

.improvement-data li {
    font-size: 1.1rem;
    line-height: 1.7;
    margin-bottom: 0.8rem;
    color: #dc2626;
    padding-left: 1.5rem;
    position: relative;
}

.improvement-data li::before {
    content: '✓';
    position: absolute;
    left: 0;
    color: #22c55e;
    font-weight: bold;
    font-size: 1.1rem;
}

.improvement-data strong {
    color: #dc2626;
    font-weight: 700;
}

.paper-link {
    display: inline-block;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    color: white;
    text-decoration: none;
    border-radius: 10px;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    width: 100%;
    text-align: center;
    box-sizing: border-box;
}

.paper-link:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* ボタン幅統一のためのコンテナ */
.button-container {
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.button-container .evidence-details,
.button-container .paper-link {
    width: 100%;
}

/* ========== セクション5専用CSS ========== */

/* 科学的根拠セクション（第2部） */
.scientific-evidence-2 {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.scientific-evidence-2 .container {
    position: relative;
    z-index: 2;
}

.scientific-evidence-2 .section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

/* 科学的コンテンツエリア */
.scientific-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* シューマン共振説明カード */
.schumann-explanation {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    text-align: center;
}

.schumann-explanation:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

.schumann-explanation > p {
    font-size: 2rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 3rem;
    color: #ff6b6b;
    text-align: center;
}

/* 研究情報エリア */
.research-info {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 15px;
    padding: 2rem;
    text-align: left;
}

.research-info h3 {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    color: #333;
    text-align: center;
    line-height: 1.3;
}

.research-info p {
    font-size: 1.2rem;
    font-weight: 500;
    line-height: 1.7;
    margin-bottom: 2rem;
    color: #666;
}

/* 統一ボタンデザイン適用 */
.research-info .paper-link {
    display: inline-block;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    color: white;
    text-decoration: none;
    border-radius: 10px;
    font-weight: 600;
    font-size: 1.1rem;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    width: 100%;
    box-sizing: border-box;
}

.research-info .paper-link:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* ========== セクション6専用CSS（二重折りたたみ構造） ========== */

/* Q&Aセクション（シューマン共振について） */
.qa-schumann {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.qa-schumann .container {
    position: relative;
    z-index: 2;
}

.qa-schumann .section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

/* Q&Aコンテンツエリア */
.qa-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* 大きなコンテナ（外側の折りたたみ） */
.qa-main-container {
    margin: 0;
}

.qa-main-container summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #4f46e5 0%, #6366f1 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(79, 70, 229, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
    margin-bottom: 2rem;
}

.qa-main-container summary::-webkit-details-marker {
    display: none;
}

.qa-main-container summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.qa-main-container[open] summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.qa-main-container summary:hover {
    background: linear-gradient(135deg, #4338ca 0%, #5b21b6 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(79, 70, 229, 0.4);
}

/* Q&Aリスト */
.qa-list {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    margin-top: 2rem;
}

/* Q&A個別アイテム */
.qa-item {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.qa-item:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 質問スタイル - センター配置 */
.qa-question {
    font-size: 1.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-bottom: 1.5rem;
    line-height: 1.4;
    text-align: center;
}

/* 回答エリア */
.qa-answer {
    margin: 0;
}

/* detailsスタイル */
.qa-answer details {
    margin: 0;
}

.qa-answer summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
}

.qa-answer summary::-webkit-details-marker {
    display: none;
}

.qa-answer summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.qa-answer details[open] summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.qa-answer summary:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* 回答コンテンツ */
.qa-answer details > *:not(summary) {
    padding: 2rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    margin-top: 1rem;
    border: 1px solid rgba(255, 107, 107, 0.1);
}

.qa-answer p {
    font-size: 1.2rem;
    font-weight: 500;
    line-height: 1.7;
    margin-bottom: 1.5rem;
    color: #666;
}

.qa-answer p:last-child {
    margin-bottom: 0;
}

/* Q&A内のh4見出し */
.qa-answer h4 {
    font-size: 1.3rem;
    font-weight: 700;
    color: #ff6b6b;
    margin: 2rem 0 1rem 0;
    border-left: 4px solid #ff6b6b;
    padding-left: 1rem;
}

/* Q&A内のリスト */
.qa-answer ul {
    list-style: none;
    padding: 0;
    margin: 1.5rem 0;
}

.qa-answer li {
    font-size: 1.1rem;
    line-height: 1.7;
    margin-bottom: 0.8rem;
    color: #666;
    padding-left: 1.5rem;
    position: relative;
}

.qa-answer li::before {
    content: '•';
    position: absolute;
    left: 0;
    color: #ff6b6b;
    font-weight: bold;
    font-size: 1.2rem;
}

.qa-answer strong {
    color: #ff6b6b;
    font-weight: 700;
}

/* ========== セクション7専用CSS（二重折りたたみ構造実装） ========== */
/* 医学的可能性セクション */
.medical-potential {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.medical-potential .container {
    position: relative;
    z-index: 2;
}

.medical-potential .section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 1.5rem;
    text-align: center;
    color: #333;
}

/* 可能性サブタイトル - レスポンシブ対応修正版 */
.potential-subtitle {
    font-size: 1.4rem;
    font-weight: 500;
    color: #666;
    text-align: center;
    margin-bottom: 2rem;
    line-height: 1.6;
}

/* 試用後画像 */
.trial-image {
    text-align: center;
    margin-bottom: 4rem;
}

.trial-image img {
    max-width: 100%;
    width: 100%;
    height: auto;
    border-radius: 15px;
    box-shadow: 0 8px 30px rgba(0, 0, 0, 0.1);
}

/* 可能性コンテンツエリア */
.potential-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* 大きなコンテナ（外側の折りたたみ） - セクション7用 */
.potential-main-container {
    margin: 0;
}

.potential-main-container summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #4f46e5 0%, #6366f1 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(79, 70, 229, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
    margin-bottom: 2rem;
}

.potential-main-container summary::-webkit-details-marker {
    display: none;
}

.potential-main-container summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.potential-main-container[open] summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.potential-main-container summary:hover {
    background: linear-gradient(135deg, #4338ca 0%, #5b21b6 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(79, 70, 229, 0.4);
}

/* 可能性グリッド */
.potential-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin: 2rem 0 4rem 0;
}

/* 可能性個別アイテム */
.potential-item {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.potential-item:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 可能性タイトル */
.potential-title {
    font-size: 1.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-bottom: 1.5rem;
    text-align: center;
    line-height: 1.3;
}

/* 可能性詳細 */
.potential-details {
    margin: 0;
}

.potential-details summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
}

.potential-details summary::-webkit-details-marker {
    display: none;
}

.potential-details summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.potential-details[open] summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.potential-details summary:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* 詳細コンテンツ */
.potential-details > p {
    padding: 2rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    margin-top: 1rem;
    border: 1px solid rgba(255, 107, 107, 0.1);
    font-size: 1.1rem;
    font-weight: 500;
    line-height: 1.7;
    color: #666;
    margin-bottom: 0;
}

/* 引用文献セクション */
.references {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.references:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

.references h3 {
    font-size: 1.8rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-bottom: 2rem;
    text-align: center;
}

.references ol {
    padding-left: 1.5rem;
}

.references li {
    font-size: 1rem;
    line-height: 1.6;
    margin-bottom: 1rem;
    color: #666;
    font-weight: 500;
}

.references li:last-child {
    margin-bottom: 0;
}

/* ========== セクション8専用CSS（統一デザインシステム適用） ========== */

/* 製品紹介セクション */
.product-intro {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.product-intro .container {
    position: relative;
    z-index: 2;
}

.product-intro .section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 2rem;
    text-align: center;
    color: #333;
}

/* 商品説明テキスト */
.product-description {
    font-size: 1.2rem;
    font-weight: 400;
    color: #666;
    line-height: 1.8;
    margin-bottom: 4rem;
    text-align: left;
    max-width: 1100px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 4rem;
}

/* 製品コンテンツエリア */
.product-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* 製品表示エリア（左右並び） */
.product-display {
    display: flex;
    align-items: flex-start;
    gap: 3rem;
    margin-bottom: 4rem;
}

/* 3Dビューアエリア */
.product-visual {
    flex: 1;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.product-visual:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* Sketchfab埋め込み */
.sketchfab-embed-wrapper {
    position: relative;
    width: 100%;
    height: 400px;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
}

.sketchfab-embed-wrapper iframe {
    width: 100%;
    height: 100%;
    border: none;
    border-radius: 15px;
}

/* 製品仕様エリア */
.product-specs {
    flex: 1;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.product-specs:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 仕様タイトル */
.specs-title {
    font-size: 1.8rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-bottom: 2rem;
    text-align: center;
    line-height: 1.3;
}

/* 仕様詳細（折りたたみ） */
.specs-details {
    margin: 0;
}

.specs-details summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
}

.specs-details summary::-webkit-details-marker {
    display: none;
}

.specs-details summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.specs-details[open] summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.specs-details summary:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* 仕様コンテンツ */
.specs-content {
    padding: 2rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    margin-top: 1rem;
    border: 1px solid rgba(255, 107, 107, 0.1);
}

/* 仕様アイテム */
.spec-item {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    padding: 1rem 0;
    border-bottom: 1px solid rgba(255, 107, 107, 0.1);
    gap: 1rem;
}

.spec-item:last-child {
    border-bottom: none;
}

.spec-label {
    font-size: 1.1rem;
    font-weight: 600;
    color: #ff6b6b;
    min-width: 120px;
    flex-shrink: 0;
}

.spec-value {
    font-size: 1.1rem;
    font-weight: 500;
    color: #666;
    line-height: 1.6;
    text-align: right;
    flex: 1;
}

/* サブタイトル */
.specs-subtitle {
    font-size: 1.4rem;
    font-weight: 700;
    color: #ff6b6b;
    margin: 2rem 0 1rem 0;
    border-left: 4px solid #ff6b6b;
    padding-left: 1rem;
}

/* ========== セクション9専用CSS（修正版） ========== */

/* 安全性セクション */
.safety-section {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.safety-section .container {
    position: relative;
    z-index: 2;
}

/* 安全性コンテンツエリア */
.safety-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* 安全性説明文（カードから外して左寄せセンター配置） */
.safety-description-text {
    font-size: 1.3rem;
    font-weight: 500;
    line-height: 1.8;
    margin-bottom: 4rem;
    color: #333;
    text-align: left;
    max-width: 900px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 4rem;
    padding: 0 20px;
}

/* 大きなコンテナ（折りたたみ機能付き） */
.safety-main-container {
    margin: 0;
}

.safety-main-container summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #4f46e5 0%, #6366f1 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(79, 70, 229, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
    margin-bottom: 2rem;
}

.safety-main-container summary::-webkit-details-marker {
    display: none;
}

.safety-main-container summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.safety-main-container[open] summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.safety-main-container summary:hover {
    background: linear-gradient(135deg, #4338ca 0%, #5b21b6 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(79, 70, 229, 0.4);
}

/* 安全性グリッド（2列表示・大きなサイズ） */
.safety-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3rem;
    margin: 2rem 0;
    max-width: 100%;
}

/* 安全性個別アイテム（大きなカードサイズ） */
.safety-item {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 3.5rem;
    text-align: center;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    min-height: 300px;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.safety-item:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 安全性比率ラベル（カードタイトルを倍に） */
.safety-ratio {
    font-size: 2.2rem;
    font-weight: 700;
    color: #333;
    margin-bottom: 2rem;
    text-align: center;
    line-height: 1.3;
}

/* 安全性タイトル（青文字・内側白文字） */
.safety-title {
    font-size: 4.5rem;
    font-weight: 800;
    margin-bottom: 2rem;
    text-align: center;
    line-height: 1.2;
    /* 青文字・内側白文字効果 */
    color: #2563eb;
    text-shadow: 
        -2px -2px 0 white,
        2px -2px 0 white,
        -2px 2px 0 white,
        2px 2px 0 white,
        0 0 4px rgba(37, 99, 235, 0.3);
    filter: drop-shadow(0 2px 4px rgba(37, 99, 235, 0.2));
}

/* 安全性説明（左詰め） */
.safety-description {
    font-size: 1.2rem;
    font-weight: 500;
    line-height: 1.7;
    color: #333;
    text-align: left;
}

/* ========== セクション10専用CSS ========== */

/* こんな方におすすめセクション */
.recommendation-section {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.recommendation-section .container {
    position: relative;
    z-index: 2;
}

/* セクションタイトル */
.recommendation-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

/* おすすめ対象者カード（PC時改行しない幅） */
.recommendation-card {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    text-align: center;
    max-width: 750px;
    margin: 0 auto 4rem;
}

.recommendation-card:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

.recommendation-list {
    list-style: none;
    padding: 0;
    text-align: left;
}

.recommendation-item {
    font-size: 1.3rem;
    font-weight: 500;
    color: #333;
    margin-bottom: 1.2rem;
    padding-left: 2rem;
    position: relative;
    line-height: 1.6;
}

.recommendation-item:last-child {
    margin-bottom: 0;
}

.recommendation-item::before {
    content: '✓';
    position: absolute;
    left: 0;
    top: 0.1rem;
    width: 1.5rem;
    height: 1.5rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    color: white;
    font-size: 0.9rem;
    box-shadow: 0 2px 8px rgba(255, 107, 107, 0.3);
}

/* 無料試用カード（変更なし） */
.trial-card {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 3rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    text-align: center;
    max-width: 900px;
    margin: 0 auto 4rem;
}

.trial-card:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

.trial-card-title {
    font-size: 2rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    color: #333;
    line-height: 1.3;
}

.trial-card-subtitle {
    font-size: 1.4rem;
    font-weight: 500;
    color: #666;
    line-height: 1.6;
}

/* フロー手順カードグリッド（1列表示） */
.flow-grid {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    max-width: 900px;
    margin: 0 auto 2rem;
}

.flow-card {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    text-align: left;
    position: relative;
}

.flow-card:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* ナンバリング：カード幅のセンター配置 */
.flow-number {
    position: absolute;
    top: -15px;
    left: 50%;
    transform: translateX(-50%);
    width: 40px;
    height: 40px;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    color: white;
    font-size: 1.2rem;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
}

/* 全画面サイズで左寄せに統一 */
.flow-card-title {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: #333;
    line-height: 1.3;
    margin-top: 0.5rem;
    text-align: left;
}

.flow-card-description {
    font-size: 1.2rem;
    font-weight: 500;
    color: #666;
    line-height: 1.6;
    margin: 0;
    text-align: left;
}

/* 注意事項テキスト */
.notice-text {
    max-width: 900px;
    margin: 0 auto 4rem;
    text-align: center;
    font-size: 1.1rem;
    font-weight: 500;
    color: #666;
    line-height: 1.6;
}

/* エンドタイトル */
.end-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.2rem;
    font-weight: 700;
    text-align: center;
    color: #ff6b6b;
    margin-top: 3rem;
    line-height: 1.4;
}

/* レスポンシブ対応 */
@media (max-width: 768px) {
    .recommendation-section {
        padding: 80px 0;
    }
    
    .recommendation-title {
        font-size: 2.2rem;
        margin-bottom: 3rem;
    }
    
    .recommendation-card {
        padding: 2rem;
        margin-bottom: 3rem;
    }
    
    .recommendation-item {
        font-size: 1.1rem;
        margin-bottom: 1rem;
    }
    
    .trial-card {
        padding: 2rem;
        margin-bottom: 3rem;
    }
    
    .trial-card-title {
        font-size: 1.6rem;
    }
    
    .trial-card-subtitle {
        font-size: 1.2rem;
    }
    
    .flow-card {
        padding: 2rem;
    }
    
    .flow-card-title {
        font-size: 1.4rem;
        margin-top: 1rem;
    }
    
    .flow-card-description {
        font-size: 1rem;
    }
    
    .notice-text {
        font-size: 1rem;
        margin-bottom: 3rem;
    }
    
    .end-title {
        font-size: 1.8rem;
        margin-top: 2rem;
    }
}

@media (max-width: 480px) {
    .recommendation-section {
        padding: 60px 0;
    }
    
    .recommendation-title {
        font-size: 1.8rem;
    }
    
    .recommendation-card {
        padding: 1.5rem;
    }
    
    .recommendation-item {
        font-size: 1rem;
        padding-left: 1.8rem;
    }
    
    .recommendation-item::before {
        width: 1.3rem;
        height: 1.3rem;
        font-size: 0.8rem;
    }
    
    .trial-card {
        padding: 1.5rem;
    }
    
    .trial-card-title {
        font-size: 1.4rem;
    }
    
    .trial-card-subtitle {
        font-size: 1.1rem;
    }
    
    .flow-card {
        padding: 1.5rem;
    }
    
    .flow-card-title {
        font-size: 1.2rem;
    }
    
    .flow-card-description {
        font-size: 0.95rem;
    }
    
    .flow-number {
        width: 35px;
        height: 35px;
        font-size: 1rem;
    }
}

@media (max-width: 320px) {
    .recommendation-title {
        font-size: 1.6rem;
    }
    
    .recommendation-item {
        font-size: 0.95rem;
    }
    
    .trial-card-title {
        font-size: 1.3rem;
    }
    
    .flow-card-title {
        font-size: 1.1rem;
    }
    
    .end-title {
        font-size: 1.6rem;
    }
}

/* ========== セクション11専用CSS（セクション6デザインベース） ========== */

/* Q&Aセクション（製品について） */
.qa-product {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.qa-product .container {
    position: relative;
    z-index: 2;
}

.qa-product .section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

/* Q&Aカードコンテナ */
.qa-cards {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

/* Q&A個別カード */
.qa-card {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.qa-card:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* カードヘッダー */
.qa-card-header {
    margin-bottom: 1.5rem;
}

/* 質問スタイル - センター配置 */
.qa-card-question {
    font-size: 1.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin: 0;
    line-height: 1.4;
    text-align: center;
}

/* カードコンテンツ */
.qa-card-content {
    margin: 0;
}

/* detailsスタイル */
.qa-details {
    margin: 0;
}

.qa-summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
}

.qa-summary::-webkit-details-marker {
    display: none;
}

.qa-summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.qa-details[open] .qa-summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.qa-summary:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* 回答コンテンツ */
.qa-answer-content {
    padding: 2rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    margin-top: 1rem;
    border: 1px solid rgba(255, 107, 107, 0.1);
}

.answer-highlight {
    font-size: 1.2rem;
    font-weight: 500;
    line-height: 1.7;
    color: #666;
    display: block;
}

/* ========== セクション12専用CSS（既存デザインに統一） ========== */

/* サブスクリプションセクション */
.subscription-section {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.subscription-section .container {
    position: relative;
    z-index: 2;
}

/* サブスクリプションコンテンツエリア */
.subscription-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* 特徴リストエリア */
.subscription-features {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    margin-bottom: 3rem;
}

.subscription-features:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 特徴アイテム */
.feature-item {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 1.8rem 2rem 1.8rem 4rem;
    margin-bottom: 1.8rem;
    position: relative;
    transition: all 0.4s ease;
    box-shadow: 0 4px 20px rgba(255, 107, 107, 0.15);
}

.feature-item:last-child {
    margin-bottom: 0;
}

.feature-item:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-4px);
    box-shadow: 0 12px 40px rgba(255, 107, 107, 0.25);
    border-color: rgba(255, 107, 107, 0.4);
}

.feature-item::before {
    content: '✓';
    position: absolute;
    left: 1rem;
    top: 50%;
    transform: translateY(-50%);
    width: 2.2rem;
    height: 2.2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    color: white;
    font-size: 1.1rem;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
}

/* 特徴ハイライトテキスト */
.feature-highlight {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
}

/* 特典セクション */
.subscription-special {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    text-align: center;
}

.subscription-special:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 特典タイトル */
.special-title {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    color: #ff6b6b;
    text-align: center;
}

/* 特典コンテンツ */
.special-content {
    margin: 0;
    text-align: center;
}

/* 特典メインタイトル（大きく表示） */
.benefit-main-title {
    font-size: 2.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-bottom: 1.5rem;
    line-height: 1.3;
}

/* 特典説明文（中サイズ） */
.benefit-description {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
    margin-bottom: 1.5rem;
}

/* 特典条件文（説明文と同じ幅になるようフォントサイズ調整） */
.benefit-condition {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
}


/* ========== セクション11専用CSS（セクション6デザインベース） ========== */

/* Q&Aセクション（製品について） */
.qa-product {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.qa-product .container {
    position: relative;
    z-index: 2;
}

.qa-product .section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

/* Q&Aカードコンテナ */
.qa-cards {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

/* Q&A個別カード */
.qa-card {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.qa-card:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* カードヘッダー */
.qa-card-header {
    margin-bottom: 1.5rem;
}

/* 質問スタイル - センター配置 */
.qa-card-question {
    font-size: 1.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin: 0;
    line-height: 1.4;
    text-align: center;
}

/* カードコンテンツ */
.qa-card-content {
    margin: 0;
}

/* detailsスタイル */
.qa-details {
    margin: 0;
}

.qa-summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
}

.qa-summary::-webkit-details-marker {
    display: none;
}

.qa-summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.qa-details[open] .qa-summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.qa-summary:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* 回答コンテンツ */
.qa-answer-content {
    padding: 2rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    margin-top: 1rem;
    border: 1px solid rgba(255, 107, 107, 0.1);
}

.answer-highlight {
    font-size: 1.2rem;
    font-weight: 500;
    line-height: 1.7;
    color: #666;
    display: block;
}

/* ========== セクション12専用CSS（既存デザインに統一） ========== */

/* サブスクリプションセクション */
.subscription-section {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.subscription-section .container {
    position: relative;
    z-index: 2;
}

/* サブスクリプションコンテンツエリア */
.subscription-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* 特徴リストエリア */
.subscription-features {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    margin-bottom: 3rem;
}

.subscription-features:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 特徴アイテム */
.feature-item {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 1.8rem 2rem 1.8rem 4rem;
    margin-bottom: 1.8rem;
    position: relative;
    transition: all 0.4s ease;
    box-shadow: 0 4px 20px rgba(255, 107, 107, 0.15);
}

.feature-item:last-child {
    margin-bottom: 0;
}

.feature-item:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-4px);
    box-shadow: 0 12px 40px rgba(255, 107, 107, 0.25);
    border-color: rgba(255, 107, 107, 0.4);
}

.feature-item::before {
    content: '✓';
    position: absolute;
    left: 1rem;
    top: 50%;
    transform: translateY(-50%);
    width: 2.2rem;
    height: 2.2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    color: white;
    font-size: 1.1rem;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
}

/* 特徴ハイライトテキスト */
.feature-highlight {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
}

/* 特典セクション */
.subscription-special {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    text-align: center;
}

.subscription-special:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 特典タイトル */
.special-title {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    color: #ff6b6b;
    text-align: center;
}

/* 特典コンテンツ */
.special-content {
    margin: 0;
    text-align: center;
}

/* 特典メインタイトル（大きく表示） */
.benefit-main-title {
    font-size: 2.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-bottom: 1.5rem;
    line-height: 1.3;
}

/* 特典説明文（中サイズ） */
.benefit-description {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
    margin-bottom: 1.5rem;
}

/* 特典条件文（説明文と同じ幅になるようフォントサイズ調整） */
.benefit-condition {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
}


/* ========== セクション11専用CSS（セクション6デザインベース） ========== */

/* Q&Aセクション（製品について） */
.qa-product {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.qa-product .container {
    position: relative;
    z-index: 2;
}

.qa-product .section-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-
    line-height: 1.4;
    margin-bottom: 4rem;
    text-align: center;
    color: #333;
}

/* Q&Aカードコンテナ */
.qa-cards {
    display: flex;
    flex-direction: column;
    gap: 2rem;
}

/* Q&A個別カード */
.qa-card {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
}

.qa-card:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* カードヘッダー */
.qa-card-header {
    margin-bottom: 1.5rem;
}

/* 質問スタイル - センター配置 */
.qa-card-question {
    font-size: 1.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin: 0;
    line-height: 1.4;
    text-align: center;
}

/* カードコンテンツ */
.qa-card-content {
    margin: 0;
}

/* detailsスタイル */
.qa-details {
    margin: 0;
}

.qa-summary {
    font-size: 1.2rem;
    font-weight: 600;
    color: white;
    cursor: pointer;
    padding: 1rem 2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 10px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    list-style: none;
    position: relative;
}

.qa-summary::-webkit-details-marker {
    display: none;
}

.qa-summary::after {
    content: '▼';
    position: absolute;
    right: 1rem;
    top: 50%;
    transform: translateY(-50%);
    transition: transform 0.3s ease;
}

.qa-details[open] .qa-summary::after {
    transform: translateY(-50%) rotate(180deg);
}

.qa-summary:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.4);
}

/* 回答コンテンツ */
.qa-answer-content {
    padding: 2rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.9) 0%, rgba(248, 249, 250, 0.95) 100%);
    border-radius: 10px;
    margin-top: 1rem;
    border: 1px solid rgba(255, 107, 107, 0.1);
}

.answer-highlight {
    font-size: 1.2rem;
    font-weight: 500;
    line-height: 1.7;
    color: #666;
    display: block;
}

/* ========== セクション12専用CSS（既存デザインに統一） ========== */

/* サブスクリプションセクション */
.subscription-section {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.subscription-section .container {
    position: relative;
    z-index: 2;
}

/* サブスクリプションコンテンツエリア */
.subscription-content {
    max-width: 1100px;
    margin: 0 auto;
}

/* 特徴リストエリア */
.subscription-features {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    margin-bottom: 3rem;
}

.subscription-features:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 特徴アイテム */
.feature-item {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 1.8rem 2rem 1.8rem 4rem;
    margin-bottom: 1.8rem;
    position: relative;
    transition: all 0.4s ease;
    box-shadow: 0 4px 20px rgba(255, 107, 107, 0.15);
}

.feature-item:last-child {
    margin-bottom: 0;
}

.feature-item:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-4px);
    box-shadow: 0 12px 40px rgba(255, 107, 107, 0.25);
    border-color: rgba(255, 107, 107, 0.4);
}

.feature-item::before {
    content: '✓';
    position: absolute;
    left: 1rem;
    top: 50%;
    transform: translateY(-50%);
    width: 2.2rem;
    height: 2.2rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
    color: white;
    font-size: 1.1rem;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
}

/* 特徴ハイライトテキスト */
.feature-highlight {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
}

/* 特典セクション */
.subscription-special {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    text-align: center;
}

.subscription-special:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

/* 特典タイトル */
.special-title {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1.5rem;
    color: #ff6b6b;
    text-align: center;
}

/* 特典コンテンツ */
.special-content {
    margin: 0;
    text-align: center;
}

/* 特典メインタイトル（大きく表示） */
.benefit-main-title {
    font-size: 2.2rem;
    font-weight: 700;
    color: #ff6b6b;
    margin-bottom: 1.5rem;
    line-height: 1.3;
}

/* 特典説明文（中サイズ） */
.benefit-description {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
    margin-bottom: 1.5rem;
}

/* 特典条件文（説明文と同じ幅になるようフォントサイズ調整） */
.benefit-condition {
    font-size: 1.54rem;
    font-weight: 500;
    color: #333;
    line-height: 1.6;
}

/* ========== セクション13専用CSS（CTAセクション） ========== */

/* CTAセクション */
.cta-section {
    background-color: white;
    color: #333;
    padding: 120px 0;
    position: relative;
    overflow: hidden;
}

.cta-section .container {
    position: relative;
    z-index: 2;
}

/* CTAコンテンツエリア */
.cta-content {
    max-width: 1100px;
    margin: 0 auto;
    text-align: center;
}

/* CTAメインタイトル */
.cta-title {
    font-family: 'Noto Sans JP', sans-serif;
    font-size: 2.8rem;
    font-weight: 700;
    line-height: 1.4;
    margin-bottom: 4rem;
    color: #333;
}

/* CTAテキストエリア */
.cta-text {
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 107, 107, 0.2);
    border-radius: 20px;
    padding: 2.5rem;
    box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
    transition: all 0.4s ease;
    margin-bottom: 4rem;
}

.cta-text:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-8px);
    box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
    border-color: rgba(255, 107, 107, 0.4);
}

.cta-text p {
    font-size: 1.3rem;
    font-weight: 500;
    line-height: 1.8;
    margin-bottom: 1.2rem;
    color: #333;
}

.cta-text p:last-child {
    margin-bottom: 0;
}

/* CTAボタンエリア */
.cta-buttons {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    max-width: 600px;
    margin: 0 auto;
}

/* メインCTAボタン */
.cta-button-main {
    display: inline-block;
    padding: 1.5rem 3rem;
    background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
    color: white;
    text-decoration: none;
    border-radius: 15px;
    font-weight: 700;
    font-size: 1.3rem;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
    text-align: center;
    position: relative;
    overflow: hidden;
}

.cta-button-main::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
    transition: left 0.5s;
}

.cta-button-main:hover {
    background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
    transform: translateY(-4px);
    box-shadow: 0 12px 35px rgba(255, 107, 107, 0.4);
}

.cta-button-main:hover::before {
    left: 100%;
}

/* サブCTAボタン - フォントサイズをメインに合わせる */
.cta-button-sub {
    display: inline-block;
    padding: 1.5rem 3rem;
    background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
    color: #ff6b6b;
    text-decoration: none;
    border: 2px solid rgba(255, 107, 107, 0.3);
    border-radius: 15px;
    font-weight: 700;
    font-size: 1.3rem;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(255, 107, 107, 0.1);
    text-align: center;
}

.cta-button-sub:hover {
    background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
    transform: translateY(-2px);
    box-shadow: 0 8px 25px rgba(255, 107, 107, 0.2);
    border-color: rgba(255, 107, 107, 0.5);
}

/* mobile-only クラス */
.mobile-only {
    display: none;
}

/* PCで画面幅が狭い場合の調整（1400px以下） */
@media (max-width: 1400px) {
    .section-title {
        font-size: 2.4rem;
    }
    
    .evidence-main-title {
        font-size: 2.4rem;
    }

    .scientific-evidence-2 .section-title {
        font-size: 2.4rem;
    }

    .qa-schumann .section-title {
        font-size: 2.4rem;
    }

    .medical-potential .section-title {
        font-size: 2.4rem;
    }

    .product-intro .section-title {
        font-size: 2.4rem;
    }

    .qa-product .section-title {
        font-size: 2.4rem;
    }

    .recommendation-title {
        font-size: 2.4rem;
    }

    .cta-title {
        font-size: 2.4rem;
    }

    .benefit-main-title {
        font-size: 2rem;
    }
    
    .device-caption {
        white-space: normal;
        line-height: 1.4;
    }
    
    .safety-item {
        padding: 3rem;
        min-height: 280px;
    }
    
    .safety-ratio {
        font-size: 2rem;
    }
    
    .safety-title {
        font-size: 4rem;
    }
}

/* より狭い画面での調整（1200px以下） */
@media (max-width: 1200px) {
    .section-title {
        font-size: 2.2rem;
    }
    
    .evidence-main-title {
        font-size: 2.2rem;
    }

    .scientific-evidence-2 .section-title {
        font-size: 2.2rem;
    }

    .qa-schumann .section-title {
        font-size: 2.2rem;
    }

    .medical-potential .section-title {
        font-size: 2.2rem;
    }

    .product-intro .section-title {
        font-size: 2.2rem;
    }

    .qa-product .section-title {
        font-size: 2.2rem;
    }

    .recommendation-title {
        font-size: 2.2rem;
    }

    .cta-title {
        font-size: 2.2rem;
    }

    .benefit-main-title {
        font-size: 1.8rem;
    }
    
    .safety-grid {
        gap: 2.5rem;
    }
    
    .safety-item {
        padding: 2.5rem;
        min-height: 260px;
    }
    
    .safety-ratio {
        font-size: 1.8rem;
    }
    
    .safety-title {
        font-size: 3.5rem;
    }
}

/* レスポンシブ対応 */
@media (max-width: 768px) {
    .mobile-only {
        display: inline;
    }

    .header-ribbon {
        height: 300px;
    }
    
    .hero, .problem-section, .solution-section, .medical-evidence-1, .scientific-evidence-2, .qa-schumann, .medical-potential, .product-intro, .safety-section, .recommendation-section, .qa-product, .subscription-section, .cta-section {
        padding: 60px 0;
    }
    
    .hero-brand {
        font-size: 2.2rem;
        margin-bottom: 1.5rem;
        letter-spacing: 0.02em;
    }
    
    .hero h1 {
        font-size: 1.8rem;
        margin-bottom: 1rem;
    }

    .problem-section h2 {
        font-size: 1.5rem;
        margin-bottom: 2rem;
        white-space: nowrap;
    }

    .problem-image {
        max-width: 100%;
        margin-bottom: 2rem;
    }
    
    .desktop-text, .section-title-desktop {
        display: none;
    }
    
    .mobile-text, .section-title-mobile {
        display: inline;
    }
    
    .hero-subtitle {
        font-size: 1rem;
        margin-bottom: 2rem;
        line-height: 1.5;
    }

    .section-title {
        font-size: 2rem;
    }

    /* セクション4スマホ改行修正 */
    .evidence-main-title {
        font-size: 2rem;
        margin-bottom: 1rem;
    }

    .evidence-main-title::after {
        content: '\A';
        white-space: pre;
    }

    .subsection-title {
        font-size: 1.3rem;
        margin-bottom: 3rem;
    }

    .subsection-title::after {
        content: '\A';
        white-space: pre;
    }

    .scientific-evidence-2 .section-title {
        font-size: 2rem;
    }

    .qa-schumann .section-title {
        font-size: 2rem;
    }

    .medical-potential .section-title {
        font-size: 2rem;
    }

    .product-intro .section-title {
        font-size: 2rem;
    }

    .qa-product .section-title {
        font-size: 2rem;
    }

    .recommendation-title {
        font-size: 2rem;
        margin-bottom: 3rem;
    }

    .cta-title {
        font-size: 2rem;
        margin-bottom: 3rem;
        text-align: left; /* スマホ時は左詰め */
    }

    /* セクション7サブタイトルのスマホ改行 */
    .potential-subtitle::after {
        content: '\A';
        white-space: pre;
    }

    .problem-list {
        padding-left: 0;
        margin-left: 1rem;
        margin-right: 1rem;
    }

    .problem-item {
        padding: 1.4rem 1.5rem 1.4rem 3.5rem;
        font-size: 1.4rem;
        margin-bottom: 1.4rem;
    }

    .problem-item::before {
        left: 0.8rem;
        width: 1.8rem;
        height: 1.8rem;
        font-size: 0.9rem;
    }

    .problem-cta {
        font-size: 1.3rem;
    }

    .content-flex {
        flex-direction: column;
        gap: 2rem;
    }

    .doctor-image {
        flex: none;
        order: -1;
        text-align: center;
        align-self: center;
        width: 100%;
    }

    .doctor-image img {
        max-width: 250px;
        margin: 0 auto;
        display: block;
    }

    .doctor-caption {
        text-align: center;
        margin: 0.5rem auto 0;
    }

    .description-card {
        text-align: left;
    }

    .description-card p {
        font-size: 1.3rem;
        line-height: 1.8;
    }

    .device-image img {
        max-width: 450px;
        margin: 1.5rem 0 1rem 0;
    }

    .device-caption-desktop {
        display: none;
    }

    .device-caption-mobile {
        display: block;
        font-size: 1rem;
        line-height: 1.4;
        white-space: normal;
    }

    .device-caption {
        font-size: 1rem;
        line-height: 1.4;
        white-space: normal;
    }

    .features-flex {
        flex-direction: column;
        gap: 2rem;
    }

    .feature-card.left-align {
        text-align: left;
    }

    .feature-card.left-align .feature-icon {
        text-align: center;
    }

    .feature-card.left-align h3 {
        text-align: center;
    }

    /* セクション4タブレット対応 */
    .evidence-cards {
        grid-template-columns: 1fr;
        gap: 2rem;
    }

    .evidence-card {
        padding: 2rem;
    }

    .card-title {
        font-size: 1.6rem;
    }

    .card-subtitle {
        font-size: 1rem;
    }

    .card-content h5 {
        font-size: 1.2rem;
    }

    .evidence-details summary {
        font-size: 1.1rem;
        padding: 0.8rem;
    }

    .improvement-data {
        padding: 1.2rem;
    }

    .improvement-data p,
    .improvement-data li {
        font-size: 1rem;
    }

    .paper-link {
        padding: 0.8rem 1.5rem;
        font-size: 1rem;
    }

    /* セクション5タブレット対応 */
    .schumann-explanation {
        padding: 2rem;
    }

    .schumann-explanation > p {
        font-size: 1.6rem;
        margin-bottom: 2.5rem;
    }

    .research-info {
        padding: 1.5rem;
    }

    .research-info h3 {
        font-size: 1.5rem;
        margin-bottom: 1.2rem;
    }

    .research-info p {
        font-size: 1.1rem;
        margin-bottom: 1.5rem;
    }

    /* セクション6タブレット対応 */
    .qa-main-container summary {
        font-size: 1.1rem;
        padding: 0.8rem 1.5rem;
    }

    .qa-item {
        padding: 2rem;
    }

    .qa-question {
        font-size: 1.1rem;
    }

    .qa-answer summary {
        font-size: 1.1rem;
        padding: 0.8rem 1.5rem;
    }

    .qa-answer details > *:not(summary) {
        padding: 1.5rem;
    }

    .qa-answer p {
        font-size: 1.1rem;
        margin-bottom: 1.2rem;
    }

    .qa-answer h4 {
        font-size: 1.2rem;
        margin: 1.5rem 0 0.8rem 0;
    }

    .qa-answer li {
        font-size: 1rem;
    }

    /* セクション7タブレット対応 */
    .potential-subtitle {
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
    }

    .trial-image {
        margin-bottom: 3rem;
    }

    .potential-main-container summary {
        font-size: 1.1rem;
        padding: 0.8rem 1.5rem;
    }

    .potential-grid {
        grid-template-columns: 1fr;
        gap: 1.5rem;
    }

    .potential-item {
        padding: 2rem;
    }

    .potential-title {
        font-size: 1.1rem;
    }

    .potential-details summary {
        font-size: 1.1rem;
        padding: 0.8rem 1.5rem;
    }

    .potential-details > p {
        padding: 1.5rem;
        font-size: 1rem;
    }

    .references {
        padding: 2rem;
    }

    .references h3 {
        font-size: 1.6rem;
        margin-bottom: 1.5rem;
    }

    .references li {
        font-size: 0.95rem;
    }

    /* セクション8タブレット対応 */
    .product-description {
        font-size: 1.1rem;
        margin-bottom: 3rem;
        padding: 0 10px;
    }

    .product-display {
        flex-direction: column;
        gap: 2rem;
        align-items: center;
    }

    .product-visual,
    .product-specs {
        flex: none;
        width: 100%;
        max-width: 500px;
        margin: 0 auto;
    }

    .sketchfab-embed-wrapper {
        height: 300px;
    }

    .spec-item {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.5rem;
    }

    .spec-label {
        min-width: auto;
    }

    .spec-value {
        text-align: left;
    }

    .specs-details summary {
        font-size: 1.1rem;
        padding: 0.8rem 1.5rem;
    }

    .specs-content {
        padding: 1.5rem;
    }

    /* セクション9タブレット対応 */
    .safety-description-text {
        font-size: 1.1rem;
        line-height: 1.6;
        padding: 0 15px;
        margin-bottom: 3rem;
        text-align: left;
    }

    .safety-grid {
        grid-template-columns: 1fr;
        gap: 2rem;
    }

    .safety-item {
        padding: 2.5rem;
        min-height: auto;
    }

    .safety-ratio {
        font-size: 1.6rem;
        margin-bottom: 1.5rem;
    }

    .safety-title {
        font-size: 3rem;
        margin-bottom: 1.5rem;
    }

    .safety-description {
        font-size: 1.1rem;
    }

    .safety-main-container summary {
        font-size: 1.1rem;
        padding: 0.8rem 1.5rem;
    }

    /* スマホ時：カード幅最大化、フォントサイズ調整 */
    .recommendation-card {
        padding: 2rem;
        margin-bottom: 3rem;
        max-width: 100%;
    }

    .recommendation-item {
        font-size: 1.05rem; /* スマホ時フォントサイズ縮小 */
        margin-bottom: 1rem;
        padding-left: 1.8rem;
    }

    .recommendation-item::before {
        width: 1.3rem;
        height:
        height: 1.3rem;
        font-size: 0.8rem;
    }

    .trial-card {
        padding: 2.5rem;
        margin-bottom: 3rem;
        max-width: 100%;
    }

    .trial-card-title {
        font-size: 1.6rem;
        margin-bottom: 1.2rem;
    }

    .trial-card-subtitle {
        font-size: 1.2rem;
    }

    .flow-grid {
        gap: 1.5rem;
        margin-bottom: 1.5rem;
        max-width: 100%;
    }

    .flow-card {
        padding: 2rem;
    }

    .flow-number {
        width: 35px;
        height: 35px;
        font-size: 1.1rem;
        top: -12px;
    }

    .flow-card-title {
        font-size: 1.4rem;
        margin-bottom: 0.8rem;
    }

    .flow-card-description {
        font-size: 1.1rem;
    }

    .notice-text {
        font-size: 0.95rem; /* スマホ時フォントサイズ縮小 */
        margin-bottom: 3rem;
        max-width: 100%;
    }

    /* スマホ時：エンドタイトル改行しないサイズ */
    .end-title {
        font-size: 1.5rem;
        margin-top: 2rem;
    }

    /* セクション11タブレット対応 */
    .qa-card {
        padding: 2rem;
    }

    .qa-card-question {
        font-size: 1.1rem;
    }

    .qa-summary {
        font-size: 1.1rem;
        padding: 0.8rem 1.5rem;
    }

    .qa-answer-content {
        padding: 1.5rem;
    }

    .answer-highlight {
        font-size: 1.1rem;
    }

    /* セクション12タブレット対応 */
    .subscription-features {
        padding: 2rem;
        margin-bottom: 2rem;
    }

    .feature-item {
        padding: 1.4rem 1.5rem 1.4rem 3.5rem;
        margin-bottom: 1.4rem;
    }

    .feature-item::before {
        left: 0.8rem;
        width: 1.8rem;
        height: 1.8rem;
        font-size: 0.9rem;
    }

    .feature-highlight {
        font-size: 1.4rem;
    }

    .subscription-special {
        padding: 2rem;
        text-align: left; /* スマホでは左詰め */
    }

    .special-title {
        font-size: 1.6rem;
        margin-bottom: 1.2rem;
        text-align: center; /* タイトルのみセンター */
    }

    .benefit-main-title {
        font-size: 1.8rem;
        text-align: center; /* メインタイトルはセンター */
    }

    .benefit-description,
    .benefit-condition {
        font-size: 1.4rem;
        text-align: left; /* 説明文は左詰め */
    }

    /* セクション13タブレット対応 */
    .cta-text {
        padding: 2rem;
        margin-bottom: 3rem;
        text-align: left; /* スマホ時は左詰め */
    }

    .cta-text p {
        font-size: 1.2rem;
        margin-bottom: 1rem;
    }

    .cta-buttons {
        gap: 1.5rem;
    }

    .cta-button-main {
        padding: 1.2rem 2rem;
        font-size: 1.1rem;
    }

    .cta-button-sub {
        padding: 1.2rem 2rem;
        font-size: 1.1rem;
    }
}

@media (max-width: 480px) {
    .header-ribbon {
        height: 250px;
    }
    
    .container, .evidence-container {
        padding: 0 15px;
    }
    
    .hero, .problem-section, .solution-section, .medical-evidence-1, .scientific-evidence-2, .qa-schumann, .medical-potential, .product-intro, .safety-section, .recommendation-section, .qa-product, .subscription-section, .cta-section {
        padding: 50px 0;
    }
    
    .hero-brand {
        font-size: 1.8rem;
        letter-spacing: 0.01em;
    }
    
    .hero h1 {
        font-size: 1.6rem;
    }

    .problem-section h2 {
        font-size: 1.3rem;
        white-space: nowrap;
    }

    .problem-image {
        margin-bottom: 1.5rem;
        border-radius: 10px;
    }
    
    .hero-subtitle {
        font-size: 0.9rem;
        padding: 0 10px;
    }

    .section-title {
        font-size: 1.6rem;
    }

    .evidence-main-title {
        font-size: 1.6rem;
    }

    .subsection-title {
        font-size: 1.1rem;
        padding: 0 10px;
    }

    .scientific-evidence-2 .section-title {
        font-size: 1.6rem;
    }

    .qa-schumann .section-title {
        font-size: 1.6rem;
    }

    .medical-potential .section-title {
        font-size: 1.6rem;
    }

    .product-intro .section-title {
        font-size: 1.6rem;
    }

    .qa-product .section-title {
        font-size: 1.6rem;
    }

    .recommendation-title {
        font-size: 1.6rem;
        margin-bottom: 2.5rem;
    }

    .cta-title {
        font-size: 1.6rem;
        margin-bottom: 2.5rem;
    }

    .problem-list {
        margin-left: 0.5rem;
        margin-right: 0.5rem;
    }

    .problem-item {
        padding: 1.2rem 1.2rem 1.2rem 3rem;
        font-size: 1.33rem;
        margin-bottom: 1.2rem;
    }

    .problem-item::before {
        left: 0.6rem;
        width: 1.6rem;
        height: 1.6rem;
        font-size: 0.8rem;
    }

    .problem-cta {
        font-size: 1.2rem;
        padding: 0 10px;
    }

    .description-card, .feature-card, .evidence-card {
        padding: 1.8rem;
    }

    .doctor-image img {
        max-width: 200px;
    }

    .device-image img {
        max-width: 375px;
        margin: 1rem 0 0.5rem 0;
    }

    .device-caption {
        font-size: 0.9rem;
        padding: 0 10px;
    }

    .feature-card h3 {
        font-size: 1.5rem;
    }

    .feature-card p {
        font-size: 1rem;
    }

    /* セクション4スマートフォン対応 */
    .evidence-cards {
        gap: 1.5rem;
    }

    .card-title {
        font-size: 1.4rem;
    }

    .card-subtitle {
        font-size: 0.95rem;
    }

    .card-content h5 {
        font-size: 1.1rem;
    }

    .evidence-details summary {
        font-size: 1rem;
        padding: 0.7rem;
    }

    .improvement-data {
        padding: 1rem;
    }

    .improvement-data p,
    .improvement-data li {
        font-size: 0.95rem;
    }

    .paper-link {
        padding: 0.7rem 1.2rem;
        font-size: 0.95rem;
    }

    /* セクション5スマートフォン対応 */
    .schumann-explanation {
        padding: 1.8rem;
    }

    .schumann-explanation > p {
        font-size: 1.4rem;
        margin-bottom: 2rem;
    }

    .research-info {
        padding: 1.2rem;
    }

    .research-info h3 {
        font-size: 1.3rem;
        margin-bottom: 1rem;
    }

    .research-info p {
        font-size: 1rem;
        margin-bottom: 1.2rem;
    }

    /* セクション6スマートフォン対応 */
    .qa-main-container summary {
        font-size: 1rem;
        padding: 0.7rem 1.2rem;
    }

    .qa-item {
        padding: 1.8rem;
    }

    .qa-question {
        font-size: 1rem;
    }

    .qa-answer summary {
        font-size: 1rem;
        padding: 0.7rem 1.2rem;
    }

    .qa-answer details > *:not(summary) {
        padding: 1.2rem;
    }

    .qa-answer p {
        font-size: 1rem;
        margin-bottom: 1rem;
    }

    .qa-answer h4 {
        font-size: 1.1rem;
        margin: 1.2rem 0 0.6rem 0;
    }

    .qa-answer li {
        font-size: 0.95rem;
    }

    /* セクション7スマートフォン対応 */
    .potential-subtitle {
        font-size: 1.1rem;
        margin-bottom: 1rem;
        padding: 0 10px;
    }

    .trial-image {
        margin-bottom: 2.5rem;
    }

    .potential-main-container summary {
        font-size: 1rem;
        padding: 0.7rem 1.2rem;
    }

    .potential-item {
        padding: 1.8rem;
    }

    .potential-title {
        font-size: 1rem;
    }

    .potential-details summary {
        font-size: 1rem;
        padding: 0.7rem 1.2rem;
    }

    .potential-details > p {
        padding: 1.2rem;
        font-size: 0.95rem;
    }

    .references {
        padding: 1.8rem;
    }

    .references h3 {
        font-size: 1.4rem;
        margin-bottom: 1.2rem;
    }

    .references li {
        font-size: 0.9rem;
    }

    /* セクション8スマートフォン対応 */
    .product-description {
        font-size: 1rem;
        margin-bottom: 2.5rem;
        padding: 0 5px;
    }

    .product-visual,
    .product-specs {
        padding: 1.8rem;
        max-width: 100%;
        width: 100%;
    }

    .sketchfab-embed-wrapper {
        height: 250px;
    }

    .specs-title {
        font-size: 1.6rem;
    }

    .specs-details summary {
        font-size: 1rem;
        padding: 0.7rem 1.2rem;
    }

    .specs-content {
        padding: 1.2rem;
    }

    .spec-label,
    .spec-value {
        font-size: 1rem;
    }

    .specs-subtitle {
        font-size: 1.2rem;
        margin: 1.5rem 0 0.8rem 0;
    }

    /* セクション9スマートフォン対応 */
    .safety-description-text {
        font-size: 1rem;
        line-height: 1.5;
        padding: 0 10px;
        margin-bottom: 2.5rem;
    }

    .safety-grid {
        gap: 1.5rem;
    }

    .safety-item {
        padding: 2rem;
    }

    .safety-ratio {
        font-size: 1.4rem;
        margin-bottom: 1.2rem;
    }

    .safety-title {
        font-size: 2.5rem;
        margin-bottom: 1.2rem;
    }

    .safety-description {
        font-size: 1rem;
    }

    .safety-main-container summary {
        font-size: 1rem;
        padding: 0.7rem 1.2rem;
    }

    .recommendation-card {
        padding: 1.8rem;
        margin-bottom: 2.5rem;
    }

    .recommendation-item {
        font-size: 0.95rem; /* さらに縮小 */
        margin-bottom: 0.8rem;
        padding-left: 1.5rem;
    }

    .recommendation-item::before {
        width: 1.2rem;
        height: 1.2rem;
        font-size: 0.7rem;
    }

    .trial-card {
        padding: 2rem;
        margin-bottom: 2.5rem;
    }

    .trial-card-title {
        font-size: 1.4rem;
        margin-bottom: 1rem;
    }

    .trial-card-subtitle {
        font-size: 1.1rem;
    }

    .flow-card {
        padding: 1.8rem;
    }

    .flow-number {
        width: 30px;
        height: 30px;
        font-size: 1rem;
        top: -10px;
    }

    .flow-card-title {
        font-size: 1.2rem;
        margin-bottom: 0.8rem;
    }

    .flow-card-description {
        font-size: 1rem;
    }

    .notice-text {
        font-size: 0.85rem; /* さらに縮小 */
        margin-bottom: 2.5rem;
    }

    .end-title {
        font-size: 1.3rem;
        margin-top: 1.5rem;
    }

    /* セクション11スマートフォン対応 */
    .qa-card {
        padding: 1.8rem;
    }

    .qa-card-question {
        font-size: 1rem;
    }

    .qa-summary {
        font-size: 1rem;
        padding: 0.7rem 1.2rem;
    }

    .qa-answer-content {
        padding: 1.2rem;
    }

    .answer-highlight {
        font-size: 1rem;
    }

    /* セクション12スマートフォン対応 */
    .subscription-features {
        padding: 1.8rem;
    }

    .feature-item {
        padding: 1.2rem 1.2rem 1.2rem 3rem;
        margin-bottom: 1.2rem;
    }

    .feature-item::before {
        left: 0.6rem;
        width: 1.6rem;
        height: 1.6rem;
        font-size: 0.8rem;
    }

    .feature-highlight {
        font-size: 1.33rem;
    }

    .subscription-special {
        padding: 1.8rem;
    }

    .special-title {
        font-size: 1.4rem;
    }

    .benefit-main-title {
        font-size: 1.6rem;
    }

    .benefit-description,
    .benefit-condition {
        font-size: 1.33rem;
    }

    /* セクション13スマートフォン対応 */
    .cta-text {
        padding: 1.8rem;
        margin-bottom: 2.5rem;
    }

    .cta-text p {
        font-size: 1.1rem;
    }

    .cta-button-main,
    .cta-button-sub {
        padding: 1rem 1.5rem;
        font-size: 1rem;
    }
}

@media (max-width: 320px) {
    .header-ribbon {
        height: 200px;
    }
    
    .hero, .problem-section, .solution-section, .medical-evidence-1, .scientific-evidence-2, .qa-schumann, .medical-potential, .product-intro, .safety-section, .recommendation-section, .qa-product, .subscription-section, .cta-section {
        padding: 40px 0;
    }
    
    .hero-brand {
        font-size: 1.5rem;
    }
    
    .hero h1 {
        font-size: 1.4rem;
    }

    .problem-section h2 {
        font-size: 1.1rem;
        white-space: nowrap;
    }

    .problem-image {
        margin-bottom: 1rem;
        border-radius: 8px;
    }
    
    .hero-subtitle {
        font-size: 0.85rem;
    }

    .section-title {
        font-size: 1.4rem;
    }

    .evidence-main-title {
        font-size: 1.4rem;
    }

    .subsection-title {
        font-size: 1rem;
        padding: 0 5px;
    }

    .scientific-evidence-2 .section-title {
        font-size: 1.4rem;
    }

    .qa-schumann .section-title {
        font-size: 1.4rem;
    }

    .medical-potential .section-title {
        font-size: 1.4rem;
    }

    .product-intro .section-title {
        font-size: 1.4rem;
    }

    .qa-product .section-title {
        font-size: 1.4rem;
    }

    .recommendation-title {
        font-size: 1.4rem;
        margin-bottom: 2rem;
    }

    .cta-title {
        font-size: 1.4rem;
        margin-bottom: 2rem;
    }

    .problem-item {
        padding: 1rem 1rem 1rem 2.5rem;
        font-size: 1.26rem;
        margin-bottom: 1rem;
    }

    .problem-item::before {
        left: 0.4rem;
        width: 1.4rem;
        height: 1.4rem;
        font-size: 0.7rem;
    }

    .problem-cta {
        font-size: 1.1rem;
    }

    .description-card, .feature-card, .evidence-card {
        padding: 1.5rem;
    }

    .device-image img {
        max-width: 300px;
        margin: 1rem 0 0.5rem 0;
    }

    .device-caption {
        font-size: 0.8rem;
        padding: 0 5px;
    }

    /* セクション4小型スマートフォン対応 */
    .card-title {
        font-size: 1.2rem;
    }

    .card-subtitle {
        font-size: 0.9rem;
    }

    .improvement-data p,
    .improvement-data li {
        font-size: 0.9rem;
    }

    .paper-link {
        padding: 0.6rem 1rem;
        font-size: 0.9rem;
    }

    /* セクション5小型スマートフォン対応 */
    .schumann-explanation {
        padding: 1.5rem;
    }

    .schumann-explanation > p {
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
    }

    .research-info {
        padding: 1rem;
    }

    .research-info h3 {
        font-size: 1.1rem;
        margin-bottom: 0.8rem;
    }

    .research-info p {
        font-size: 0.9rem;
        margin-bottom: 1rem;
    }

    /* セクション6小型スマートフォン対応 */
    .qa-main-container summary {
        font-size: 0.9rem;
        padding: 0.6rem 1rem;
    }

    .qa-item {
        padding: 1.5rem;
    }

    .qa-question {
        font-size: 0.9rem;
    }

    .qa-answer summary {
        font-size: 0.9rem;
        padding: 0.6rem 1rem;
    }

    .qa-answer details > *:not(summary) {
        padding: 1rem;
    }

    .qa-answer p {
        font-size: 0.9rem;
        margin-bottom: 0.8rem;
    }

    .qa-answer h4 {
        font-size: 1rem;
        margin: 1rem 0 0.5rem 0;
    }

    .qa-answer li {
        font-size: 0.9rem;
    }

    /* セクション7小型スマートフォン対応 */
    .potential-subtitle {
        font-size: 1rem;
        margin-bottom: 0.8rem;
        padding: 0 5px;
    }

    .trial-image {
        margin-bottom: 2rem;
    }

    .potential-main-container summary {
        font-size: 0.9rem;
        padding: 0.6rem 1rem;
    }

    .potential-item {
        padding: 1.5rem;
    }

    .potential-title {
        font-size: 0.9rem;
    }

    .potential-details summary {
        font-size: 0.9rem;
        padding: 0.6rem 1rem;
    }

    .potential-details > p {
        padding: 1rem;
        font-size: 0.9rem;
    }

    .references {
        padding: 1.5rem;
    }

    .references h3 {
        font-size: 1.2rem;
        margin-bottom: 1rem;
    }

    .references li {
        font-size: 0.85rem;
    }

    /* セクション8小型スマートフォン対応 */
    .product-description {
        font-size: 0.9rem;
        margin-bottom: 2rem;
        padding: 0;
    }

    .product-visual,
    .product-specs {
        padding: 1.5rem;
    }

    .sketchfab-embed-wrapper {
        height: 200px;
    }

    .specs-title {
        font-size: 1.4rem;
    }

    .specs-details summary {
        font-size: 0.9rem;
        padding: 0.6rem 1rem;
    }

    .specs-content {
        padding: 1rem;
    }

    .spec-label,
    .spec-value {
        font-size: 0.9rem;
    }

    .specs-subtitle {
        font-size: 1.1rem;
        margin: 1.2rem 0 0.6rem 0;
    }

    /* セクション9小型スマートフォン対応 */
    .safety-description-text {
        font-size: 0.95rem;
        line-height: 1.4;
        padding: 0 5px;
        margin-bottom: 2rem;
    }

    .safety-item {
        padding: 1.5rem;
    }

    .safety-ratio {
        font-size: 1.2rem;
        margin-bottom: 1rem;
    }

    .safety-title {
        font-size: 2.2rem;
        margin-bottom: 1rem;
    }

    .safety-description {
        font-size: 0.95rem;
    }

    .safety-main-container summary {
        font-size: 0.9rem;
        padding: 0.6rem 1rem;
    }

    .recommendation-card {
        padding: 1.5rem;
        margin-bottom: 2rem;
    }

    .recommendation-item {
        font-size: 0.85rem; /* 最小サイズ */
        margin-bottom: 0.7rem;
        padding-left: 1.3rem;
    }

    .recommendation-item::before {
        width: 1rem;
        height: 1rem;
        font-size: 0.6rem;
    }

    .trial-card {
        padding: 1.5rem;
        margin-bottom: 2rem;
    }

    .trial-card-title {
        font-size: 1.2rem;
        margin-bottom: 0.8rem;
    }

    .trial-card-subtitle {
        font-size: 1rem;
    }

    .flow-card {
        padding: 1.5rem;
    }

    .flow-number {
        width: 28px;
        height: 28px;
        font-size: 0.9rem;
        top: -8px;
    }

    .flow-card-title {
        font-size: 1.1rem;
        margin-bottom: 0.6rem;
    }

    .flow-card-description {
        font-size: 0.9rem;
    }

    .notice-text {
        font-size: 0.75rem; /* 最小サイズ */
        margin-bottom: 2rem;
    }

    .end-title {
        font-size: 1.1rem;
        margin-top: 1rem;
    }

    /* セクション11小型スマートフォン対応 */
    .qa-card {
        padding: 1.5rem;
    }

    .qa-card-question {
        font-size: 0.9rem;
    }

    .qa-summary {
        font-size: 0.9rem;
        padding: 0.6rem 1rem;
    }

    .qa-answer-content {
        padding: 1rem;
    }

    .answer-highlight {
        font-size: 0.9rem;
    }

    /* セクション12小型スマートフォン対応 */
    .subscription-features {
        padding: 1.5rem;
    }

    .feature-item {
        padding: 1rem 1rem 1rem 2.5rem;
        margin-bottom: 1rem;
    }

    .feature-item::before {
        left: 0.4rem;
        width: 1.4rem;
        height: 1.4rem;
        font-size: 0.7rem;
    }

    .feature-highlight {
        font-size: 1.26rem;
    }

    .subscription-special {
        padding: 1.5rem;
    }

    .special-title {
        font-size: 1.2rem;
    }

    .benefit-main-title {
        font-size: 1.4rem;
    }

    .benefit-description,
    .benefit-condition {
        font-size: 1.26rem;
    }

    /* セクション13小型スマートフォン対応 */
    .cta-text {
        padding: 1.5rem;
        margin-bottom: 2rem;
    }

    .cta-text p {
        font-size: 1rem;
    }

    .cta-button-main,
    .cta-button-sub {
        padding: 0.8rem 1.2rem;
        font-size: 0.95rem;
    }
}

<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Synchro Wave 01 - セクション13 CTA</title>
    
    <!-- フォント読み込み -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&family=Noto+Sans+JP:wght@400;500;700&display=swap" rel="stylesheet">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Noto Sans JP', sans-serif;
            line-height: 1.6;
            background-color: white;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

       /* ========== セクション13専用CSS（CTAセクション） ========== */
        
        /* CTAセクション */
        .cta-section {
            background-color: white;
            color: #333;
            padding: 120px 0;
            position: relative;
            overflow: hidden;
        }

        .cta-section .container {
            position: relative;
            z-index: 2;
        }

        /* CTAコンテンツエリア */
        .cta-content {
            max-width: 1100px;
            margin: 0 auto;
            text-align: center;
        }

        /* CTAメインタイトル */
        .cta-title {
            font-family: 'Noto Sans JP', sans-serif;
            font-size: 2.8rem;
            font-weight: 700;
            line-height: 1.4;
            margin-bottom: 4rem;
            color: #333;
        }

        /* CTAテキストエリア */
        .cta-text {
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
            backdrop-filter: blur(20px);
            border: 2px solid rgba(255, 107, 107, 0.2);
            border-radius: 20px;
            padding: 2.5rem;
            box-shadow: 0 8px 32px rgba(255, 107, 107, 0.1);
            transition: all 0.4s ease;
            margin-bottom: 4rem;
        }

        .cta-text:hover {
            background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
            transform: translateY(-8px);
            box-shadow: 0 16px 48px rgba(255, 107, 107, 0.15);
            border-color: rgba(255, 107, 107, 0.4);
        }

        .cta-text p {
            font-size: 1.3rem;
            font-weight: 500;
            line-height: 1.8;
            margin-bottom: 1.2rem;
            color: #333;
        }

        .cta-text p:last-child {
            margin-bottom: 0;
        }

        /* CTAボタンエリア */
        .cta-buttons {
            display: flex;
            flex-direction: column;
            gap: 2rem;
            max-width: 600px;
            margin: 0 auto;
        }

        /* メインCTAボタン */
        .cta-button-main {
            display: inline-block;
            padding: 1.5rem 3rem;
            background: linear-gradient(135deg, #ff6b6b 0%, #ff8e8e 100%);
            color: white;
            text-decoration: none;
            border-radius: 15px;
            font-weight: 700;
            font-size: 1.3rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .cta-button-main::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s;
        }

        .cta-button-main:hover {
            background: linear-gradient(135deg, #ff5252 0%, #ff7575 100%);
            transform: translateY(-4px);
            box-shadow: 0 12px 35px rgba(255, 107, 107, 0.4);
        }

        .cta-button-main:hover::before {
            left: 100%;
        }

        /* サブCTAボタン - フォントサイズをメインに合わせる */
        .cta-button-sub {
            display: inline-block;
            padding: 1.5rem 3rem;
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.95) 0%, rgba(248, 249, 250, 0.9) 100%);
            color: #ff6b6b;
            text-decoration: none;
            border: 2px solid rgba(255, 107, 107, 0.3);
            border-radius: 15px;
            font-weight: 700;
            font-size: 1.3rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.1);
            text-align: center;
        }

        .cta-button-sub:hover {
            background: linear-gradient(135deg, rgba(255, 255, 255, 1) 0%, rgba(255, 245, 245, 1) 100%);
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(255, 107, 107, 0.2);
            border-color: rgba(255, 107, 107, 0.5);
        }

        /* レスポンシブ対応 */
        @media (max-width: 768px) {
            .cta-section {
                padding: 60px 0;
            }

            .cta-title {
                font-size: 2rem;
                margin-bottom: 3rem;
                text-align: left; /* スマホ時は左詰め */
            }

            .cta-text {
                padding: 2rem;
                margin-bottom: 3rem;
                text-align: left; /* スマホ時は左詰め */
            }

            .cta-text p {
                font-size: 1.2rem;
                margin-bottom: 1rem;
            }

            .cta-buttons {
                gap: 1.5rem;
            }

            .cta-button-main {
                padding: 1.2rem 2rem;
                font-size: 1.1rem;
            }

            .cta-button-sub {
                padding: 1.2rem 2rem;
                font-size: 1.1rem;
            }
        }
        @media (max-width: 320px) {
            .cta-section {
                padding: 40px 0;
            }

            .cta-title {
                font-size: 1.4rem;
                margin-bottom: 2rem;
            }

            .cta-text {
                padding: 1.5rem;
                margin-bottom: 2rem;
            }

            .cta-text p {
                font-size: 1rem;
            }

            .cta-button-main,
            .cta-button-sub {
                padding: 0.8rem 1.2rem;
                font-size: 0.95rem;
            }
        }
    </style>
</head>
<body>

    </style>
</head>
<body>
    <!-- ヘッダーリボン -->
    <div class="header-ribbon"></div>
    
    <!-- 1. メインタイトル・サブタイトルセクション -->
    <section class="hero">
        <div class="container">
            <div class="hero-brand">SYNCHRO WAVE 01</div>
            <h1>
                <span class="desktop-text">睡眠医学の権威が立案した<br>新しい睡眠改善サポートをあなたに</span>
                <span class="mobile-text">睡眠医学の権威が立案した<br>新しい睡眠改善サポートを<br>あなたに</span>
            </h1>
            <p class="hero-subtitle">医学的根拠のあるサポートで「眠りの質」は良くなります</p>
        </div>
    </section>

    <!-- 2. 問題提起セクション -->
    <section class="problem-section">
        <div class="container">
            <h2>このような睡眠の悩み、ありませんか？</h2>
            
            <!-- 問題定義用画像を追加 -->
            <img src="https://i.imgur.com/jgALWIl.png" alt="睡眠の悩み" class="problem-image">
            
            <ul class="problem-list">
                <li class="problem-item">夜中に何度も目が覚める</li>
                <li class="problem-item">深い眠りに入れず、朝まで熟睡できない日が多い</li>
                <li class="problem-item">朝すっきり起きられない</li>
                <li class="problem-item">十分な睡眠時間を取っているのに、疲れが取れない、昼間の眠気が酷い</li>
                <li class="problem-item">薬以外の方法で睡眠を改善したい</li>
                <li class="problem-item">体に負担の少ない方法で、夜間のトイレの回数を少なくしたい</li>
                <li class="problem-item">信頼できる情報が欲しい</li>
            </ul>
            <p class="problem-cta">医師と睡眠改善に取り組みませんか？</p>
        </div>
    </section>

    <!-- 3. 新しい睡眠サポートセクション -->
    <section class="solution-section">
        <div class="container">
            <h2 class="section-title">
                <span class="section-title-desktop">睡眠医学の権威クリスチャン・ギルミノー医学博士が立案</span>
                <span class="section-title-mobile">睡眠医学の権威<br>クリスチャン・ギルミノー医学博士が立案</span>
            </h2>
            
            <!-- 説明文と博士画像の横並び -->
            <div class="content-flex">
                <div class="description-card">
                    <p>不眠症患者の睡眠改善のために、クリスチャン・ギルミノー医学博士はこれまでにないアプローチを立案しました。それが、この特別なデバイスを用いた「新しい睡眠改善サポート」です。そして、デバイスの鍵となるのが、地球の鼓動と言われる「シューマン共振」です。</p>
                </div>
                <div class="doctor-image">
                    <img src="https://imgur.com/1Ja1iPE.jpg" alt="クリスチャン・ギルミノー医学博士">
                    <p class="doctor-caption">クリスチャン・ギルミノー医学博士</p>
                </div>
            </div>

            <!-- シューマン共振発信器画像 + キャプション修正 -->
            <div class="device-image">
                <img src="https://imgur.com/9XkrB1m.jpg" alt="シューマン共振発信器">
                <p class="device-caption">
                    <span class="device-caption-desktop">クリスチャン・ギルミノー医学博士が開発した睡眠デバイス（特許出願済）</span>
                    <span class="device-caption-mobile">クリスチャン・ギルミノー医学博士が開発した睡眠デバイス<br><span style="float: right;">（特許出願済）</span></span>
                </p>
            </div>

            <!-- 特徴カード（左右並び） -->
            <div class="features-flex">
                <div class="feature-card">
                    <span class="feature-icon">🌍</span>
                    <h3>地球の鼓動</h3>
                    <p>シューマン共振（7.83Hz）は<span class="desktop-text">地球と電離層の間で発生する自然の電磁波</span><span class="mobile-text">地球と電離層の間で発生<br>する自然の電磁波</span>。人間の脳波と同調する周波数です。</p>
                </div>
                <div class="feature-card left-align">
                    <span class="feature-icon">🛏️</span>
                    <h3>簡単設置</h3>
                    <p>ベッドサイドに置くだけ。特別な操作は不要で、自然に睡眠環境が整います。</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 4. 医学的根拠セクション（スマホ改行修正版） -->
    <section class="medical-evidence-1" id="medical-evidence-1">
        <div class="evidence-container">
            <h2 class="evidence-main-title">シューマン共振と睡眠改善の<br class="mobile-only">関係性</h2>
            <h3 class="subsection-title">臨床試験データが示す<br class="mobile-only">「新しい睡眠改善サポート」の効果</h3>
            
            <div class="evidence-cards">
                <!-- 不眠症改善効果カード -->
                <article class="evidence-card">
                    <header class="card-header">
                        <h4 class="card-title">不眠症改善効果</h4>
                        <p class="card-subtitle">睡眠医学の権威クリスチャン・ギルミノー医学博士が立案し、Huang, Yu-Shu医学博士が実施した不眠症患者に実施した非侵襲的治療</p>
                    </header>
                    <div class="card-content">
                        <h5>臨床試験が示す改善データ</h5>
                        <div class="button-container">
                            <details class="evidence-details">
                                <summary>詳細を見る</summary>
                                <div class="improvement-data">
                                    <ul>
                                        <li>シューマン共振を利用した非侵襲的治療で、被験者の78%が主観的・客観的に睡眠の質が改善</li>
                                        <li><strong>入眠時間30%短縮</strong> - 平均45分→32分に改善</li>
                                        <li><strong>中途覚醒回数半減</strong> - 夜間の目覚める回数が大幅減少</li>
                                        <li><strong>深睡眠時間の延長</strong> - より質の高い睡眠を実現</li>
                                        <li><strong>朝の目覚めの改善</strong> - スッキリとした起床感を報告</li>
                                    </ul>
                                </div>
                            </details>
                            <a href="https://www.dovepress.com/the-subjective-and-objective-improvement-of-non-invasive-treatment-of--peer-reviewed-fulltext-article-NSS" class="paper-link" target="_blank" rel="noopener">臨床試験論文を読む</a>
                        </div>
                    </div>
                </article>

                <!-- 夜間頻尿患者の睡眠改善効果カード -->
                <article class="evidence-card">
                    <header class="card-header">
                        <h4 class="card-title">夜間頻尿患者の睡眠改善効果</h4>
                        <p class="card-subtitle">Huang, Yu-Shu医学博士が夜間頻尿患者に実施した非侵襲的治療</p>
                    </header>
                    <div class="card-content">
                        <h5>臨床試験が示す改善データ</h5>
                        <div class="button-container">
                            <details class="evidence-details">
                                <summary>詳細を見る</summary>
                                <div class="improvement-data">
                                    <p>電磁場曝露により夜間トイレ回数が平均2.3回→1.1回に減少。深睡眠時間が1.5倍に増加</p>
                                    <ul>
                                        <li><strong>夜間排尿回数52%減少</strong> - 2.3回から1.1回へ大幅改善</li>
                                        <li><strong>深睡眠時間1.5倍増加</strong> - より深い睡眠段階の延長</li>
                                        <li><strong>睡眠効率の向上</strong> - 全体的な睡眠の質が改善</li>
                                        <li><strong>日中の活動性向上</strong> - 夜間の睡眠改善により昼間の生活の質が向上</li>
                                    </ul>
                                </div>
                            </details>
                            <a href="https://journals.lww.com/md-journal/fulltext/2022/08120/the_effect_of_electromagnetic_field_on_sleep_of.82.aspx" class="paper-link" target="_blank" rel="noopener">臨床試験論文を読む</a>
                        </div>
                    </div>
                </article>
            </div>
        </div>
    </section>

    <!-- 5. 科学的根拠セクション（第2部） -->
    <section class="scientific-evidence-2" id="scientific-evidence-2">
        <div class="container">
            <h2 class="section-title">シューマン共振とは</h2>
            <div class="scientific-content">
                <div class="schumann-explanation">
                    <p><span class="desktop-text">地球と電離層の間で発生する自然の電磁波共振</span><span class="mobile-text">地球と電離層の間で発生<br>する自然の電磁波共振</span></p>
                    <div class="research-info">
                        <h3><span class="desktop-text">京都大学基礎物理学研究所 村瀬雅俊博士の研究</span><span class="mobile-text">京都大学基礎物理学研究所<br><span style="text-align: center; display: block;">村瀬雅俊博士の研究</span></span></h3>
                        <p>シューマン共振が脳波（アルファ波やシータ波）に似ており、セロトニンやメラトニンの分泌に影響を与える可能性が実験データを通じて科学的に評価</p>
                        <a href="https://dl.ndl.go.jp/view/prepareDownload?itemId=info%3Andljp%2Fpid%2F10940777&contentNo=1" class="paper-link" target="_blank" rel="noopener">論文を読む</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 6. Q&Aセクション（シューマン共振について） - 二重折りたたみ構造 -->
    <section class="qa-schumann" id="qa-schumann">
        <div class="container">
            <h2 class="section-title">シューマン共振について</h2>
            <div class="qa-content">
                <details class="qa-main-container">
                    <summary>詳しく見る</summary>
                    <dl class="qa-list">
                        <div class="qa-item">
                            <dt class="qa-question">Q1. シューマン共振とは何ですか？</dt>
                            <dd class="qa-answer">
                                <details>
                                    <summary>詳細</summary>
                                    <p>シューマン共振は、地球の表面と電離層の間の空洞で発生する自然の超低周波（ELF）電磁波現象です。主な周波数は7.83Hzで、「地球の鼓動」とも呼ばれています。雷放電によって常に励起されており、地球全体に広がる自然のリズムです。</p>
                                </details>
                            </dd>
                        </div>

                        <div class="qa-item">
                            <dt class="qa-question">Q2. シューマン共振と低周波音はどう違うのですか？</dt>
                            <dd class="qa-answer">
                                <details>
                                    <summary>詳細</summary>
                                    <p>シューマン共振は、電場と磁場が組み合わさって空間を波のように伝わる電磁波の一種です。地球の表面と電離層の間で発生する自然の超低周波電磁波現象で、主な周波数は7.83Hzです。一方、低周波音は、人間が聞き取りにくい20Hz以下の周波数を持つ空気の振動、すなわち音波の一種です。これは体で感じたり、不快感や健康被害の原因となることがあり、シューマン共振とは発生源も性質も全く異なるものです。</p>
                                </details>
                            </dd>
                        </div>

                        <div class="qa-item">
                            <dt class="qa-question">Q3. 自然界の電磁波と人工電磁波はどう違うのですか？</dt>
                            <dd class="qa-answer">
                                <details>
                                    <summary>詳細</summary>
                                    <p>自然界の電磁波は、地球の磁場や雷、太陽光など、生物が進化の過程で適応してきたものです。一方、人工電磁波は近年急速に増えたもので、周波数や強度、波形が多様です。生体への影響は、自然界のものと人工のものとで異なる可能性があります。</p>
                                </details>
                            </dd>
                        </div>

                        <div class="qa-item">
                            <dt class="qa-question">Q4. 脳波とシューマン共振の類似しているのですか？</dt>
                            <dd class="qa-answer">
                                <details>
                                    <summary>詳細</summary>
                                    <p>はい、脳波とシューマン共振には顕著な類似性があります。</p>
                                    <h4>1. 周波数範囲の重複</h4>
                                    <ul>
                                        <li><strong>シータ波領域（4-8Hz）</strong>: シューマン共振の基本周波数7.83Hzが、人間のシータ波帯域と完全に一致</li>
                                        <li><strong>ベータ波領域（12-30Hz）</strong>: シューマン共振の14.3Hz、20.8Hzがベータ波帯域内に位置</li>
                                        <li><strong>ガンマ波領域（>30Hz）</strong>: シューマン共振の27.3Hz、33.8Hz、45Hzがガンマ波帯域と対応</li>
                                    </ul>
                                    <h4>2. 機能的な対応関係</h4>
                                    <ul>
                                        <li><strong>7.83Hz</strong>: リラクゼーション・創造性状態と地球の基本共振周波数が一致</li>
                                        <li><strong>高周波数帯</strong>: 高レベルの情報処理（ガンマ波）とシューマン共振の高次モードが対応</li>
                                    </ul>
                                    <h4>3. 生理学的意義</h4>
                                    <p>この類似性は偶然ではなく、人間の脳が地球の電磁環境に適応して進化してきた結果と考えられています。特に、最も安定したシューマン共振の基本周波数7.83Hzが、リラクゼーションや創造性に関連するシータ波帯域と一致することは、人間の意識状態と地球環境の深い関連性を示唆しています。</p>
                                </details>
                            </dd>
                        </div>

                        <div class="qa-item">
                            <dt class="qa-question">Q5. シューマン共振は健康にどんな影響がありますか？</dt>
                            <dd class="qa-answer">
                                <details>
                                    <summary>詳細</summary>
                                    <p>シューマン共振の周波数は人の脳波（シータ波・アルファ波）と重なっており、睡眠やストレス、気分、認知機能などに良い影響を与える可能性が国内外の研究で示唆されています。睡眠の質改善やストレス軽減などの報告もあり、今後の研究が期待される分野です。</p>
                                </details>
                            </dd>
                        </div>

                        <div class="qa-item">
                            <dt class="qa-question">Q6. シューマン共振で有害事象は起こりますか？</dt>
                            <dd class="qa-answer">
                                <details>
                                    <summary>詳細</summary>
                                    <p>不眠症観察研究46名の参加者のうち、2名がデバイス使用中に頭痛とめまいを経験（1名はSR睡眠デバイス群、もう1名はプラセボデバイス群）、その他の有害事象は認められませんでした。</p>
                                    <p>夜間頻尿観察研究35名の参加者のうち、2名がデバイス使用中に頭痛とめまいを経験（1名はSR睡眠デバイス群、もう1名はプラセボデバイス群）、その他の有害事象は認められませんでした。</p>
                                </details>
                            </dd>
                        </div>
                    </dl>
                </details>
            </div>
        </div>
    </section>

    <!-- 7. 医学的可能性セクション（二重折りたたみ構造実装） -->
    <section class="medical-potential" id="medical-potential">
        <div class="container">
            <h2 class="section-title">シューマン共振の可能性</h2>
            <p class="potential-subtitle">シューマン共振は睡眠以外にも<br class="mobile-only">健康に良い影響があります</p>
            
            <!-- 医学的可能性セクション画像を追加 -->
            <div class="trial-image">
                <img src="https://imgur.com/NWKk95c.png" alt="シューマン共振の可能性" class="problem-image">
            </div>
            
            <div class="potential-content">
                <details class="potential-main-container">
                    <summary>詳しく見る</summary>
                    <div class="potential-grid">
                        <div class="potential-item">
                            <h3 class="potential-title">睡眠</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>シューマン共振への曝露や、地球の電磁場と身体を繋げるグラウンディング（アーシング）が、睡眠の質の改善に繋がる可能性が示唆されています。シューマン共振は、睡眠や気分に関わるセロトニン/メラトニンバランスに影響を与える可能性のある生物物理学的メカニズムとして提案されています。<br>引用 [[1]](#__1), [[2]](#__2), [[3]](#__3), [[7]](#__7) より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">ストレス</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>2018年の研究では、シューマン共振への曝露がストレスを軽減する可能性が示されました。また、グラウンディングも炎症を軽減し、ストレスや不安を軽減することが示唆されており、シューマン共振との繋がりが考えられています。<br>引用 [[2]](#__2), [[3]](#__3) より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">気分</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>シューマン共振への曝露が気分の改善に繋がる可能性が示唆されています。これは、シューマン共振がセロトニン/メラトニンバランスに影響を与える可能性のある生物物理学的メカニズムとして提案されていることと関連があると考えられます。ただし、ELF場によるメラトニン減少の知見もあり、さらなる調査が必要です。<br>引用 [[1]](#__1) より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">認知機能（記憶力、集中力）</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>2017年の研究では、シューマン共振への曝露が、記憶力や集中力の向上を含む、ヒトの認知機能および身体能力にプラスの影響を与える可能性が示唆されています。特に、アルファ波（8-12 Hz）の範囲にあるシューマン共振の周波数が、リラックスした覚醒状態や認知処理と関連があると考えられています。<br>引用 [[1]](#__1) より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">痛み</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>シューマン共振周波数を用いた治療により、痛みや睡眠障害を持つ患者において主観的および客観的な改善が観察されています。これは、シューマン共振周波数が潜在的な治療応用を持つ可能性を示唆しています。<br>引用 [[6]](#__6) より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">炎症</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>動物実験（マウス）において、シューマン共振の高調波である15 Hzの周波数での反復経頭蓋磁気刺激が、炎症を軽減する可能性が示されました。<br>引用 [[2]](#__2) より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">抑うつ症状</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>動物実験（マウス）において、シューマン共振の高調波である15 Hzの周波数での反復経頭蓋磁気刺激が、抑うつ症状を軽減する可能性が示されました。</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">心筋細胞の損傷</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>動物実験（ラット心筋）において、シューマン共振の基本周波数に近い7.8 Hzの周波数で90 nTの磁場を印加したところ、H₂O₂によって誘発された心筋細胞の損傷を約40％減少させる有益な効果が観察されました。<br>引用 [4] より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">血圧</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>グラウンディング（アーシング）による地球の電磁場との接続が血圧の改善に寄与する可能性が示唆されており、シューマン共振との関連性が考えられています。自律神経系への影響を通じて、血圧調節に良い影響を与える可能性があります。<br>引用 [3] より</p>
                            </details>
                        </div>

                        <div class="potential-item">
                            <h3 class="potential-title">免疫機能</h3>
                            <details class="potential-details">
                                <summary>詳細を見る</summary>
                                <p>シューマン共振が免疫系に影響を与える可能性が理論的に提案されています。電磁場が細胞レベルでの生理学的プロセスに影響を与えることで、免疫機能の調節に寄与する可能性があります。ただし、この分野はまだ研究が限られており、さらなる調査が必要です。<br>引用 [5] より</p>
                            </details>
                        </div>
                    </div>
            <!-- 引用文献セクション -->
            <div class="references">
                <h3>引用文献</h3>
                <ol>
                    <li id="__1">Huang, Y. S., Guilleminault, C., Hwang, F. M., Cheng, C., Lin, C. H., Li, H. Y., & Lee, L. A. (2022). The subjective and objective improvement of non-invasive treatment of insomnia in adults. Nature and Science of Sleep, 14, 1905-1920.</li>
                    <li id="__2">Huang, Y. S., Guilleminault, C., Lin, C. H., Hwang, F. M., Liu, C. J., & Yang, C. M. (2022). The effect of electromagnetic field on sleep of patients with nocturia. Medicine, 101(33), e30084.</li>
                    <li id="__3">Chevalier, G., Sinatra, S. T., Oschman, J. L., Sokal, K., & Sokal, P. (2012). Earthing: health implications of reconnecting the human body to the Earth's surface electrons. Journal of environmental and public health, 2012.</li>
                    <li id="__4">Persinger, M. A. (2014). Infrasound, human health, and adaptation: an integrative overview of recondite hazards in a complex environment. Natural hazards, 70(1), 501-525.</li>
                    <li id="__5">Saroka, K. S., Persinger, M. A., & Koren, S. A. (2013). The electromagnetic induction of mystical experiences: experimental approach and neurobiological implications. Journal of Consciousness Exploration & Research, 4(7).</li>
                    <li id="__6">Ghaly, M., & Teplitz, D. (2004). The biologic effects of grounding the human body during sleep as measured by cortisol levels and subjective reporting of sleep, pain, and stress. The Journal of Alternative & Complementary Medicine, 10(5), 767-776.</li>
                    <li id="__7">村瀬雅俊. (2003). シューマン共振と生体への影響に関する研究. 京都大学基礎物理学研究所研究報告.</li>
                </ol>
            </div>
        </div>
    </section>

    <!-- 8. 製品紹介セクション -->
    <section class="product-intro" id="product-intro">
        <div class="container">
            <h2 class="section-title">製品紹介</h2>
            <p class="product-description">
                Synchrowave01はクリスチャン･ギルミノー医学博士の検証実験に着想を得て開発した、超小型ELF超低周波共振波発信器です。自然界と同調する周波数を精密に発信します。
            </p>
            
            <div class="product-content">
                <div class="product-display">
                    <!-- 3Dビューア -->
                    <div class="product-visual">
                        <div class="sketchfab-embed-wrapper">
                            <iframe 
                               title="Synchro Wave 01" 
                               frameborder="0" 
                               allowfullscreen 
                                mozallowfullscreen="true" 
                                webkitallowfullscreen="true" 
                                allow="autoplay; fullscreen; xr-spatial-tracking" 
                                xr-spatial-tracking 
                                execution-while-out-of-viewport 
                                execution-while-not-rendered 
                                web-share 
                                src="https://sketchfab.com/models/5f94e3abf69943db9276d864d35d89aa/embed?autostart=1&ui_controls=1&ui_infos=1&ui_inspector=1&ui_stop=1&ui_watermark=1&ui_watermark_link=1">
                            </iframe>
                        </div>
                    </div>
                    <!-- 製品仕様 -->
                    <div class="product-specs">
                        <h3 class="specs-title">製品仕様</h3>
                        <details class="specs-details">
                            <summary>仕様データを見る</summary>
                            <div class="specs-content">
                                <div class="spec-item">
                                    <div class="spec-label">サイズ・重量</div>
                                    <div class="spec-value">56×56×12mm / 39g</div>
                                </div>
                                <div class="spec-item">
                                    <div class="spec-label">デバイス種別</div>
                                    <div class="spec-value">ELF超低周波共振波発信器</div>
                                </div>
                                <div class="spec-item">
                                    <div class="spec-label">特徴</div>
                                    <div class="spec-value">手のひらサイズの超小型デバイスで、自然界と同調する周波数を精密に発信します</div>
                                </div>
                                
                                <h4 class="specs-subtitle">主要機能</h4>
                                <div class="spec-item">
                                    <div class="spec-label">発信周波数</div>
                                    <div class="spec-value">シューマン共振(7.83Hz)を中心とした周波数発信</div>
                                </div>
                                <div class="spec-item">
                                    <div class="spec-label">周波数範囲</div>
                                    <div class="spec-value">0.01Hz～9999Hz（純粋な正弦波）</div>
                                </div>
                                <div class="spec-item">
                                    <div class="spec-label">デフォルト設定</div>
                                    <div class="spec-value">7.83Hz（シューマン共振）</div>
                                </div>
                                <div class="spec-item">
                                    <div class="spec-label">電源</div>
                                    <div class="spec-value">USB Type-C（スマートフォン用充電器対応）</div>
                                </div>
                                <div class="spec-item">
                                    <div class="spec-label">消費電力</div>
                                    <div class="spec-value">0.085 W（省電力設計）</div>
                                </div
                            </div>
                        </details>
                    </div>
                </div>
            </div>
        </div>
    </section>

    
                    </div>
                </details>
            </div>
        </div>
    </section>
   <!-- 11. Q&Aセクション（製品について） -->
    <section class="qa-product" id="qa-product">
        <div class="container">
            <h2 class="section-title">Synchro Wave 01についてQ&A</h2>
            <div class="qa-content">
                <div class="qa-cards">
                    <!-- Q1カード -->
                    <div class="qa-card">
                        <div class="qa-card-header">
                            <h3 class="qa-card-question">Q1: 「Synchro Wave 01」は医療機器ですか？</h3>
                        </div>
                        <div class="qa-card-content">
                            <details class="qa-details">
                                <summary class="qa-summary">回答を見る</summary>
                                <div class="qa-answer-content">
                                    <span class="answer-highlight">いいえ、「Synchro Wave 01」は医療機器ではありません。ELF超低周波発信器です。治療や予防を目的としたものではありません。</span>
                                </div>
                            </details>
                        </div>
                    </div>

                    <!-- Q2カード -->
                    <div class="qa-card">
                        <div class="qa-card-header">
                            <h3 class="qa-card-question">Q2: 効果はすぐに現れますか？</h3>
                        </div>
                        <div class="qa-card-content">
                            <details class="qa-details">
                                <summary class="qa-summary">回答を見る</summary>
                                <div class="qa-answer-content">
                                    <span class="answer-highlight">ELF超低周波発信器の感じ方には個人差があります。数日で変化を感じる方もいらっしゃれば、数週間かけて徐々に変化を感じる方もいらっしゃいます。まずは60日間の無料体験期間を通じて、じっくりとお試しください。</span>
                                </div>
                            </details>
                        </div>
                    </div>

                    <!-- Q3カード -->
                    <div class="qa-card">
                        <div class="qa-card-header">
                            <h3 class="qa-card-question">Q3: どのような人におすすめですか？</h3>
                        </div>
                        <div class="qa-card-content">
                            <details class="qa-details">
                                <summary class="qa-summary">回答を見る</summary>
                                <div class="qa-answer-content">
                                    <span class="answer-highlight">睡眠の質に課題を感じている方、薬に頼らず睡眠環境を改善したい方、日中のパフォーマンスを高めたい方などにおすすめです。ただし、禁忌事項に該当する方や、重篤な睡眠障害をお持ちの方は、必ず医師にご相談ください。</span>
                                </div>
                            </details>
                        </div>
                    </div>

                    <!-- Q4カード -->
                    <div class="qa-card">
                        <div class="qa-card-header">
                            <h3 class="qa-card-question">Q4: 使用する上で副作用はありますか？</h3>
                        </div>
                        <div class="qa-card-content">
                            <details class="qa-details">
                                <summary class="qa-summary">回答を見る</summary>
                                <div class="qa-answer-content">
                                    <span class="answer-highlight">シューマン共振の先行研究では、プラセボ群と同程度の軽微な有害事象（頭痛、めまいなど）が報告されていますが、シューマン共振特有の重篤な副作用は報告されていません。ご使用中に何か異変を感じた場合は、直ちに使用を中止し、医師にご相談ください。</span>
                                </div>
                            </details>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <script>
        // 折りたたみ要素のアニメーション強化
        document.querySelectorAll('details').forEach(details => {
            details.addEventListener('toggle', function() {
                if (this.open) {
                    // 開く時のアニメーション
                    const content = this.querySelector('summary').nextElementSibling;
                    if (content) {
                        content.style.animation = 'fadeInSlideDown 0.3s ease-out';
                    }
                }
            });
        });

        // フェードインアニメーション用のキーフレーム（CSS）
        const style = document.createElement('style');
        style.textContent = `
            @keyframes fadeInSlideDown {
                from {
                    opacity: 0;
                    transform: translateY(-10px);
                }
                to {
                    opacity: 1;
                    transform: translateY(0);
                }
            }
        `;
        document.head.appendChild(style);

        // パフォーマンス最適化：Intersection Observer for lazy loading
        const observerOptions = {
            root: null,
            rootMargin: '50px',
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('animate-in');
                }
            });
        }, observerOptions);

        // アニメーション対象要素を監視
        document.querySelectorAll('.qa-card').forEach(el => {
            observer.observe(el);
        });
    </script>

</body> 
   <!-- セクション9: 安全性セクション -->
    <section class="safety-section" id="safety">
        <div class="container">
            <h2 class="section-title">synchrowave01の安全性評価</h2>
            
            <!-- 安全性説明文（カード外・左寄せセンター配置） -->
            <div class="safety-description-text">
                Synchro Wave 01は、日本と国際安全基準すべてを大幅に下回る極めて安全なELF超低周波発信器です。自然界に存在するシューマン共振と同じ周波数を、正確に安定して発信できる設計となっています。
            </div>
            
            <div class="safety-content">
                <!-- 大きなコンテナ（折りたたみ機能） -->
                <details class="safety-main-container">
                    <summary>安全性を見る</summary>
                    <div class="safety-grid">
                        <div class="safety-item">
                            <div class="safety-ratio">地球磁場との比較</div>
                            <h3 class="safety-title">1/21</h3>
                            <p class="safety-description">地球の磁場（約 24,000 nT ～ 66,000 nT）に対し 1140 nT程度の極めて低い磁束密度</p>
                        </div>

                        <div class="safety-item">
                            <div class="safety-ratio">誘導電場</div>
                            <h3 class="safety-title">1/166667</h3>
                            <p class="safety-description">自然界の電場（100V/m）に対し0.000006V/m自然界の電場と比較して、極めて低い値</p>
                        </div>

                        <div class="safety-item">
                            <div class="safety-ratio">国際基準との比較</div>
                            <h3 class="safety-title">1/200000</h3>
                            <p class="safety-description">ICNIRP国際非電離放射線防護委員会の基準数百 V/ｍに対し 0.0000063 V/m 基準を大幅に下回っている</p>
                        </div>

                        <div class="safety-item">
                            <div class="safety-ratio">生体への影響</div>
                            <h3 class="safety-title">1/158730</h3>
                            <p class="safety-description">電場強度が 1 V/m 以下では生体への影響はほとんどないのに対し 0.0000063 V/m であり、人体への影響は無視できるレベル</p>
                        </div>
                    </div>
                </details>
            </div>
        </div>
    </section>
    <!-- 10. こんな方におすすめセクション -->
    <section class="recommendation-section" id="recommendation-section">
        <div class="container">
            <h2 class="recommendation-title">こんな方におすすめ</h2>
            
            <!-- おすすめ対象者カード（PC時改行しない幅） -->
            <div class="recommendation-card">
                <ul class="recommendation-list">
                    <li class="recommendation-item">睡眠の質を本気で改善したい方</li>
                    <li class="recommendation-item">投薬以外の方法で睡眠をサポートしたい方</li>
                    <li class="recommendation-item">睡眠時無呼吸症候群、歯ぎしり、いびき等の治療中の方</li>
                    <li class="recommendation-item">企業の健康経営や生産性向上を目指す経営者</li>
                </ul>
            </div>

            <!-- 無料試用カード（変更なし） -->
            <div class="trial-card">
                <h3 class="trial-card-title">60日間効果を感じるまで無料で試すことができます</h3>
                <p class="trial-card-subtitle">まずはじっくりと効果を実感していただけます</p>
            </div>

            <!-- フロー手順カードグリッド（1列表示） -->
            <div class="flow-grid">
                <div class="flow-card">
                    <div class="flow-number">1</div>
                    <h4 class="flow-card-title">医師または歯科医師によるヒアリング・ご説明</h4>
                    <p class="flow-card-description">専門医があなたの睡眠状況を詳しくお聞きし、製品について丁寧にご説明いたします。</p>
                </div>

                <div class="flow-card">
                    <div class="flow-number">2</div>
                    <h4 class="flow-card-title">あなたに最適な周波数を設定</h4>
                    <p class="flow-card-description">個人の状態に合わせて、最適な周波数設定を行います。</p>
                </div>

                <div class="flow-card">
                    <div class="flow-number">3</div>
                    <h4 class="flow-card-title">ベッドサイドに置くだけ・電源はスマホの充電器でOK</h4>
                    <p class="flow-card-description">設置は簡単。お手持ちのスマートフォン充電器で動作します。</p>
                </div>

                <div class="flow-card">
                    <div class="flow-number">4</div>
                    <h4 class="flow-card-title">60日間じっくり効果を実感</h4>
                    <p class="flow-card-description">無料体験期間中に、睡眠の質の変化をじっくりとお確かめください。</p>
                </div>

                <div class="flow-card">
                    <div class="flow-number">5</div>
                    <h4 class="flow-card-title">睡眠サポートを継続する場合はご契約、効果を感じなければ貸出機を返却</h4>
                    <p class="flow-card-description">効果を実感いただけた場合のみ継続。満足いただけない場合は無料で返却可能です。</p>
                </div>

                <div class="flow-card">
                    <div class="flow-number">6</div>
                    <h4 class="flow-card-title">契約期間中フォローアップで睡眠の最適化を継続</h4>
                    <p class="flow-card-description">継続期間中も定期的なフォローアップで、より良い睡眠環境をサポートします。</p>
                </div>
            </div>

            <!-- 注意事項テキスト -->
            <div class="notice-text">
                ※販売ではなく、サブスクリプション契約（月額3,500円）です。<br>
                ※契約・決済は診療所を通じて行います。
            </div>

            <!-- エンドタイトル -->
            <h3 class="end-title">医師と睡眠改善に取り組みませんか？</h3>
        </div>
    </section>
            <!-- エンドタイトル -->
            <h3 class="end-title">質の高い睡眠で、より良い毎日を</h3>
        </div>
    </section>
</body>
<!-- 12. サブスクリプションセクション -->
    <section class="subscription-section" id="subscription">
        <div class="container">
            <h2 class="section-title">サブスクリプションプラン</h2>
            <div class="subscription-content">
                <div class="subscription-features">
                    <div class="feature-item">
                        <span class="feature-highlight">Synchro Wave 01は販売ではなく貸与システム</span>
                    </div>
                    <div class="feature-item">
                        <span class="feature-highlight">月額3,500円（税込）のサブスクリプション契約です。</span>
                    </div>
                    <div class="feature-item">
                        <span class="feature-highlight">60日間無料体験 - 効果を実感してからご契約いただけます。</span>
                    </div>
                    <div class="feature-item">
                        <span class="feature-highlight">違約金なし - いつでも解約可能です。</span>
                    </div>
                    <div class="feature-item">
                        <span class="feature-highlight">医師によるサポート - 継続的な睡眠指導を受けられます。</span>
                    </div>
                    <div class="feature-item">
                        <span class="feature-highlight">メンテナンス込み - 故障時は無償交換いたします。</span>
                    </div>
                    <div class="feature-item">
                        <span class="feature-highlight">バージョンアップ対応 - 新技術への無償アップデートも対応します。</span>
                    </div>
                </div>

                <div class="subscription-special">
                    <h3 class="special-title">特典</h3>
                    <div class="special-content">
                        <div class="benefit-main-title">60日間完全無料体験</div>
                        <div class="benefit-description">上質な睡眠を安定して実感いただける平均期間（60日）は完全無料</div>
                        <div class="benefit-condition">効果を感じられない場合は費用は一切かかりません。</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <script>
        // スムーズスクロール機能
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // ホバーエフェクト強化
        document.querySelectorAll('.feature-item, .subscription-special').forEach(item => {
            item.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-4px)';
            });
            
            item.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0)';
            });
        });

        // パフォーマンス最適化：Intersection Observer for animations
        const observerOptions = {
            root: null,
            rootMargin: '50px',
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('animate-in');
                }
            });
        }, observerOptions);

        // アニメーション対象要素を監視
        document.querySelectorAll('.feature-item, .subscription-special').forEach(el => {
            observer.observe(el);
        });
    </script>

</body>
 <!-- 13. CTAセクション -->
    <section class="cta-section" id="cta">
        <div class="container">
            <div class="cta-content">
                <h2 class="cta-title">上質な睡眠への第一歩を踏み出しませんか？</h2>
                <div class="cta-text">
                    <p>もう、眠れない夜に悩む必要はありません。</p>
                    <p>医師と共に、科学的根拠に基づいた睡眠改善を始めましょう。</p>
                    <p>まずは60日間の無料体験で良質な眠りを実感してください。</p>
                </div>
                
                <div class="cta-buttons">
                    <a href="#trial" class="cta-button-main">
                        60日間無料体験を始める
                    </a>
                    <a href="#manual" class="cta-button-sub">
                        synchrowave01の取扱説明書を見る
                    </a>
                </div>
            </div>
        </div>
    </section>

    <script>
        // CTAボタンのクリックイベント
        document.querySelectorAll('.cta-button-main, .cta-button-sub').forEach(button => {
            button.addEventListener('click', function(e) {
                e.preventDefault();
                
                // ボタンクリック時のアニメーション
                this.style.transform = 'scale(0.95)';
                setTimeout(() => {
                    this.style.transform = '';
                }, 150);
                
                // 実際のリンク処理（必要に応じて実装）
                console.log('CTA button clicked:', this.textContent);
            });
        });

        // スクロールアニメーション
        const observerOptions = {
            root: null,
            rootMargin: '50px',
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // 初期状態設定とアニメーション監視
        document.querySelectorAll('.cta-text').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(30px)';
            el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(el);
        });
    </script>
</body>
</html>

            }
        }
</html>

</html>
