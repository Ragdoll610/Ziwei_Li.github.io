---
layout: project-detail
title: 制御回路
permalink: /projects/project5
---

<h1>モータードライバ</h1>

<div class="jp-title-box">
  1）KEA
</div>

<style>
  table.custom-table {
    width: 100%;
    border-collapse: collapse;
    border: 1px solid #ccc;
    text-align: left;
  }

  table.custom-table th,
  table.custom-table td {
    border: 1px solid #ccc;
    padding: 0.5em 1em;
  }

  table.custom-table tbody tr:nth-child(even) td:not(:first-child) {
    background-color: #f9f9f9;
  }

  table.custom-table tbody tr:nth-child(odd) td:not(:first-child) {
    background-color: #eeeeee;
  }
</style>

<p>本研究では…（此处省略）...</p>

<p>
  <img src="{{ site.baseurl }}/images/project5.svg"
       alt="System Overview"
       style="max-width: 100%; height: auto; display: block; margin: auto;">
</p>


<h3>回路図に使用した主な部品一覧</h3>

<table class="custom-table">
  <thead>
    <tr>
      <th>カテゴリ</th>
      <th>型番 / 名称</th>
      <th>数量</th>
      <th>機能の説明</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="3"><strong>IC</strong></td>
      <td>MC34063</td>
      <td>1</td>
      <td>昇圧型DC-DCスイッチングレギュレータ</td>
    </tr>
    <tr>
      <td>74HC573</td>
      <td>1</td>
      <td>8ビットラッチ、パラレル出力制御用</td>
    </tr>
    <tr>
      <td>IR2104</td>
      <td>2</td>
      <td>ハイ・ローサイドMOSFETドライバ、Hブリッジ制御用</td>
    </tr>

    <tr>
      <td><strong>MOSFET</strong></td>
      <td>NチャネルMOSFET（例：IRF540N）</td>
      <td>4</td>
      <td>Hブリッジ構成、双方向負荷（モーターなど）制御</td>
    </tr>

    <tr>
      <td rowspan="2"><strong>ダイオード</strong></td>
      <td>IN5819（ショットキーダイオード）</td>
      <td>6</td>
      <td>整流、フリーホイール、逆電流保護</td>
    </tr>
    <tr>
      <td>LED（0805）</td>
      <td>1</td>
      <td>電源インジケータ</td>
    </tr>

    <tr>
      <td><strong>抵抗</strong></td>
      <td>各種抵抗（例：0.22Ω、10kΩ、33Ω）</td>
      <td>17</td>
      <td>分圧、電流制限、電流検出など</td>
    </tr>

    <tr>
      <td><strong>コンデンサ</strong></td>
      <td>各種（例：220μF、150pF、470μF）</td>
      <td>7</td>
      <td>フィルタ、安定化、カップリング・デカップリング</td>
    </tr>

    <tr>
      <td><strong>インダクタ</strong></td>
      <td>330μH</td>
      <td>1</td>
      <td>昇圧回路のエネルギー蓄積用</td>
    </tr>

    <tr>
      <td><strong>コネクタ</strong></td>
      <td>ソケット / ピンヘッダ（SIP2）</td>
      <td>4</td>
      <td>電源、信号、負荷用の接続端子</td>
    </tr>
  </tbody>
</table>
