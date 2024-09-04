
Cara alternatif ambil Query_id atau User_id pada telegram desktop bisa copy kemudian dipaste ke webdev console (jangan lupa aktifkan paste pada console dengan ketik "allow pasting"), Gunakan salah satu method dibawah ini.

✳️Method 1
  ```
let value = sessionStorage.getItem('__telegram__initParams');
let params = JSON.parse(value);
let tgWebAppData = params.tgWebAppData;
copy(tgWebAppData);
console.log("Success copy QueryID / UserID");
 ```
✳️Method 2 (Jika method 1 tidak bisa)
 ```
let value = sessionStorage.getItem('telegram-apps/launch-params');
let params = new URLSearchParams(value);
let tgWebAppData = params.get('tgWebAppData');
copy(tgWebAppData);
console.log("Success copy QueryID / UserID");
 ```
📝 Query_id atau User_id otomatis ter-copy dan jika ada symbol (") diakhir Query_id atau User_id silahkan di delete saja
