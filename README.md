
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Boulevard-Projectr</title>

  <!-- Google Analytics -->
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-DXNB3EZL75"></script>
  <script>
    console.log("✅ Google Analytics script is running...");  

    window.dataLayer = window.dataLayer || [];
    function gtag(){ dataLayer.push(arguments); }

    gtag('js', new Date());
    gtag('config', 'G-DXNB3EZL75', { 'debug_mode': true });

    // Get the current date and time
    const currentDate = new Date();
    const formattedDate = currentDate.toISOString();  // ISO format

    // Get the page title and path
    const pageTitle = document.title;  // Will fetch the title of the current page
    const pagePath = window.location.pathname;  // Will fetch the path of the current page (e.g., /somepage)

    // Track Page View with additional details
    gtag('event', 'page_view', {
      'page_path': pagePath,
      'page_title': pageTitle,  // Explicitly sending page title
      'view_date': formattedDate
    });

    // Check if Google Analytics is initialized
    setTimeout(() => {
      console.log("🔍 Checking dataLayer:", window.dataLayer);
    }, 2000);
  </script>
  <!-- End Google Analytics -->

  <style>
    body {
      margin: 0;
      padding: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f4f4f4;
    }
    iframe {
      width: 100%;
      height: 100vh;
      border: none;
    }
  </style>
</head>
<body>

  <!-- Power BI Report Embed -->
  <iframe title="بروتوتيب البوليفارد(داخلي)" 
  src="https://app.powerbi.com/view?r=eyJrIjoiNGFiZDQ4ZGItNjBkYy00ZjJjLTk2OTMtYjJkZDg5MGQ3NTVjIiwidCI6ImM3YmNkYzYzLTI4M2MtNDk5OC05NTk0LTQ1NTM5MzNlNGQ1YiIsImMiOjl9" 
  allowFullScreen="true">
  
  </iframe>
</body>
</html>
