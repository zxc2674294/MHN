<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>座標表</title>
</head>
<body>
  <table>
    <tr>
      <th>座標</th>
      <th>描述</th>
    </tr>
    <tr>
      <td>120, 120</td>
      <td>台北 101</td>
    </tr>
    <tr>
      <td>25.027567, 121.569192</td>
      <td>高雄 85 大樓</td>
    </tr>
    <tr>
      <td>23.697689, 120.979287</td>
      <td>台中 101</td>
    </tr>
  </table>

  <button id="copy-coordinates">複製座標</button>

  <script>
    document.getElementById("copy-coordinates").addEventListener("click", function() {
      var table = document.querySelector("table");
      var coordinates = [];
      for (var i = 0; i < table.rows.length; i++) {
        var row = table.rows[i];
        coordinates.push(row.cells[0].textContent + ", " + row.cells[1].textContent);
      }
      var clipboard = new ClipboardJS();
      clipboard.writeText(coordinates.join("\n"));
    });
  </script>
</body>
</html>
