const http = require('http');

const port = process.env.PORT || 3000;

const server = http.createServer((req, res) => {

  res.statusCode = 200;

  res.setHeader('Content-Type', 'text/html; charset=utf-8');

  res.end('<h1>สวัสดีครับ! นี่คือ Web Server ของ นางสาว อารียา พันธ์เพ็ชร</h1><p>เครื่องแม่ข่ายทำงานปกติบนระบบ Railway แล้วครับผม!</p>');
});

server.listen(port, () => {
  console.log(`Server is running! เครื่องแม่ข่ายเปิดทำงานแล้วที่ช่องทาง: ${port}`);
});
