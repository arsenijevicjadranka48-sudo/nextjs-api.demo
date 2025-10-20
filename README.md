<!DOCTYPE html>
<html lang="sr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MCA2017 – Mašinska obrada</title>
<style>
body { font-family: Arial, sans-serif; margin:0; padding:0; background:#f9f9f9; color:#222; scroll-behavior:smooth; }
header { display: flex; justify-content: space-between; align-items: center; padding: 10px 20px; position: relative; background:#333; color:white; }
header .left { display: flex; align-items: center; gap: 10px; }
header .right { display: flex; align-items: center; gap: 15px; position: relative; }
nav { display: flex; gap: 15px; }
nav a { color:white; text-decoration:none; font-weight:bold; }
nav a:hover { text-decoration: underline; }

.lang-container {
  opacity: 0;             
  transition: opacity 0.3s ease;
  display: flex;
  gap: 5px;
  align-items: center;
}
header .right:hover .lang-container {
  opacity: 1;             
}

.lang-btn { 
  padding: 5px 10px; 
  border:none; 
  border-radius:5px; 
  cursor:pointer; 
  background:#555; 
  color:white; 
  display: flex;
  align-items: center;
  gap: 5px;
}
.lang-btn.active
