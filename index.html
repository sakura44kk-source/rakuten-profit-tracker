<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>楽天リサーチツール（安全版）</title>

<style>
body {
    font-family: sans-serif;
    background: #f5f5f5;
    padding: 20px;
}

.container {
    max-width: 500px;
    margin: auto;
}

.card {
    background: white;
    padding: 16px;
    border-radius: 12px;
    margin-bottom: 16px;
}

input, button {
    width: 100%;
    padding: 10px;
    margin-top: 8px;
}

button {
    background: #ff7eb3;
    color: white;
    border: none;
    cursor: pointer;
}

.product {
    border-bottom: 1px solid #ddd;
    padding: 8px 0;
}
</style>
</head>

<body>

<div class="container">

<div class="card">
<h3>APIキー入力</h3>
<input type="text" id="appId" placeholder="楽天ApplicationID">
</div>

<div class="card">
<h3>商品検索</h3>
<input type="text" id="keyword" placeholder="例：シルバニア">
<button onclick="search()">検索</button>
</div>

<div class="card">
<h3>結果</h3>
<div id="results"></div>
</div>

</div>

<script>

async function search() {
    const appId = document.getElementById('appId').value.trim();
    const keyword = document.getElementById('keyword').value.trim();

    if (!appId) {
        alert('APIキー入れて');
        return;
    }

    if (!keyword) {
        alert('キーワード入れて');
        return;
    }

    const url = `https://openapi.rakuten.co.jp/services/api/IchibaItem/Search/20220601?format=json&keyword=${encodeURIComponent(keyword)}&hits=20&applicationId=${appId}`;

    try {
        const res = await fetch(url);
        const data = await res.json();

        const results = document.getElementById('results');
        results.innerHTML = '';

        if (!data.Items) {
            results.innerHTML = '結果なし';
            return;
        }

        data.Items.forEach(i => {
            const item = i.Item;

            const div = document.createElement('div');
            div.className = 'product';
            div.innerHTML = `
                <div><b>${item.itemName}</b></div>
                <div>¥${item.itemPrice}</div>
                <a href="${item.itemUrl}" target="_blank">開く</a>
            `;

            results.appendChild(div);
        });

    } catch (e) {
        alert('エラー：' + e.message);
    }
}

</script>

</body>
</html>
