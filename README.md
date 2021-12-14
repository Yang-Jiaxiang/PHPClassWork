# PHPClassWork

<h2>OpenData抓取空氣汙染<h2>
  爬取網頁
  $json =file_get_contents('https://data.epa.gov.tw/api/v1/aqx_p_432?limit=1000&api_key=9be7b239-557b-4c10-9775-78cadfc555e9&sort=ImportDate%20desc&format=json');
  
  處理Json
  $obj=json_decode($json, true);
  
  算數量
  $count = count($obj["records"]);
