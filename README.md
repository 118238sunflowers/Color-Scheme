# Color-Scheme
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Sunflower Sunset Color Scheme</title>
  <style>
    :root{
      --name-font: Georgia, "Times New Roman", serif;       /* used for color names */
      --value-font: "Helvetica Neue", Helvetica, Arial, sans-serif; /* used for hex/rgb/hsl values */
    }

    body{
      margin: 24px;
      font-family: var(--value-font);
      background: linear-gradient(180deg, #fffaf0, #ffeef8);
      color: #222;
    }

    table.color-table{
      width: 100%;
      max-width: 900px;
      border-collapse: collapse;
      box-shadow: 0 6px 18px rgba(0,0,0,0.08);
      margin: 0 auto;
      border-radius: 8px;
      overflow: hidden;
    }

    /* Header: the color scheme title (uses fonts from other text in the table) */
    thead th.scheme-title{
      background: linear-gradient(90deg, rgba(255,195,0,0.95), rgba(74,144,226,0.95));
      color: #fff;
      text-align: left;
      padding: 18px 20px;
      font-size: 1.15rem;
      /* header uses both fonts used elsewhere (one or more font styles from table text) */
      font-family: var(--name-font), var(--value-font);
      font-weight: 700;
      letter-spacing: 0.2px;
    }

    thead th.scheme-title span.subtitle{
      display:block;
      font-weight:400;
      font-size:0.85rem;
      opacity:0.95;
      margin-top:6px;
      font-family: var(--value-font);
    }

    thead th:not(.scheme-title){
      padding: 12px 14px;
      text-align: left;
    }

    tbody td{
      padding: 14px 16px;
      border-right: 1px solid rgba(255,255,255,0.06);
      vertical-align: middle;
      font-size: 0.95rem;
    }

    /* Column widths */
    col.name { width: 25%; }
    col.hex  { width: 25%; }
    col.rgb  { width: 25%; }
    col.hsl  { width: 25%; }

    /* Color name text style */
    td.color-name{
      font-family: var(--name-font);
      font-weight: 600;
      font-size: 1rem;
      text-shadow: 0 1px 0 rgba(255,255,255,0.12);
    }

    /* Values use the value font */
    td.value{
      font-family: var(--value-font);
      font-weight: 500;
      font-size: 0.92rem;
      opacity: 0.98;
    }

    /* Make sure table cells don't wrap color codes awkwardly */
    td.value code{
      white-space:nowrap;
      font-family: Menlo, Monaco, Consolas, "Courier New", monospace;
      background: rgba(255,255,255,0.06);
      padding: 2px 6px;
      border-radius: 4px;
      display:inline-block;
    }

    /* Small caption area under the table for notes */
    .note{
      max-width:900px;
      margin: 10px auto 0;
      font-size:0.9rem;
      color:#444;
      text-align:left;
      font-family:var(--value-font);
    }

    /* Responsive */
    @media (max-width:640px){
      thead th.scheme-title{ font-size:1rem; padding:14px; }
      tbody td{ padding:12px; font-size:0.92rem; }
    }
  </style>
</head>
<body>

  <table class="color-table" aria-describedby="scheme-note" role="table">
    <colgroup>
      <col class="name" />
      <col class="hex" />
      <col class="rgb" />
      <col class="hsl" />
    </colgroup>

    <thead>
      <tr>
        <!-- Header is the scheme title (table header) -->
        <th class="scheme-title" colspan="4" scope="col">
          Sunflower Sunset Color Scheme
          <span class="subtitle">Sunflowers (yellow, brown) + Sunset (pink, blue)</span>
        </th>
      </tr>
      <tr>
        <th style="padding:10px 16px; text-align:left; font-weight:700;">Color name</th>
        <th style="padding:10px 16px; text-align:left; font-weight:700;">Hex</th>
        <th style="padding:10px 16px; text-align:left; font-weight:700;">RGB</th>
        <th style="padding:10px 16px; text-align:left; font-weight:700;">HSL</th>
      </tr>
    </thead>

    <tbody>
      <!-- Sunflower Yellow -->
      <tr>
        <td class="color-name" style="background-color:#FFC300; color:#000;">
          Sunflower Yellow
        </td>
        <td class="value" style="background-color:#FFC300; color:#000;">
          <code>#FFC300</code>
        </td>
        <td class="value" style="background-color:#FFC300; color:#000;">
          <code>rgb(255, 195, 0)</code>
        </td>
        <td class="value" style="background-color:#FFC300; color:#000;">
          <code>hsl(46, 100%, 50%)</code>
        </td>
      </tr>

      <!-- Sunflower Brown (center/seed color) -->
      <tr>
        <td class="color-name" style="background-color:#8B5A2B; color:#fff;">
          Sunflower Brown
        </td>
        <td class="value" style="background-color:#8B5A2B; color:#fff;">
          <code>#8B5A2B</code>
        </td>
        <td class="value" style="background-color:#8B5A2B; color:#fff;">
          <code>rgb(139, 90, 43)</code>
        </td>
        <td class="value" style="background-color:#8B5A2B; color:#fff;">
          <code>hsl(29, 53%, 36%)</code>
        </td>
      </tr>

      <!-- Sunset Pink -->
      <tr>
        <td class="color-name" style="background-color:#FF6F91; color:#000;">
          Sunset Pink
        </td>
        <td class="value" style="background-color:#FF6F91; color:#000;">
          <code>#FF6F91</code>
        </td>
        <td class="value" style="background-color:#FF6F91; color:#000;">
          <code>rgb(255, 111, 145)</code>
        </td>
        <td class="value" style="background-color:#FF6F91; color:#000;">
          <code>hsl(346, 100%, 72%)</code>
        </td>
      </tr>

      <!-- Sunset Blue -->
      <tr>
        <td class="color-name" style="background-color:#4A90E2; color:#fff;">
          Sunset Blue
        </td>
        <td class="value" style="background-color:#4A90E2; color:#fff;">
          <code>#4A90E2</code>
        </td>
        <td class="value" style="background-color:#4A90E2; color:#fff;">
          <code>rgb(74, 144, 226)</code>
        </td>
        <td class="value" style="background-color:#4A90E2; color:#fff;">
          <code>hsl(212, 72%, 59%)</code>
        </td>
      </tr>
    </tbody>
  </table>

</body>
</html>
