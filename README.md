# sainiwalaa-website-
<div id="app"></div>

<style>
:root{
  --amazon:#FFD814;
  --flipkart:#2874F0;
  --bg:#f1f3f6;

  /* 🔥 SHEET CONTROLLED */
  --product-text-color:#000000;
}

body{
  margin:0;
  background:var(--bg);
  font-family:Poppins,Arial,sans-serif;
}

/* CONTAINER */
.offer-wrapper{
  max-width:1400px;
  margin:0 auto;
  padding:20px;
}

/* TITLE */
.offer-title{
  text-align:center;
  font-size:28px;
  font-weight:700;
  margin-bottom:25px;
  color:#111;
}

/* CATEGORY BAR */
.cat-bar{
  display:flex;
  flex-wrap:wrap;
  gap:12px;
  justify-content:center;
  margin-bottom:30px;
}

.cat-btn{
  padding:10px 20px;
  border-radius:25px;
  border:none;
  background:#fff;
  font-weight:600;
  cursor:pointer;
  box-shadow:0 4px 10px rgba(0,0,0,.15);
}

.cat-btn.active{
  background:var(--flipkart);
  color:#fff;
}

/* GRID */
.product-grid{
  display:grid;
  grid-template-columns:repeat(4, minmax(0,1fr));
  gap:22px;
}

@media(max-width:1200px){
  .product-grid{ grid-template-columns:repeat(3,1fr); }
}
@media(max-width:768px){
  .product-grid{ grid-template-columns:repeat(2,1fr); }
}

/* CARD */
.product-card{
  background:#fff;
  border-radius:16px;
  box-shadow:0 8px 22px rgba(0,0,0,.15);
  padding:15px;
  display:flex;
  flex-direction:column;
  position:relative;
}

/* IMAGE */
.product-card img{
  width:100%;
  height:260px;
  object-fit:contain;
}

/* BADGES */
.badge-top{
  position:absolute;
  top:10px;
  left:10px;
  background:#b12704;
  color:#fff;
  padding:5px 8px;
  font-size:12px;
  border-radius:6px;
}

.badge-off{
  position:absolute;
  top:10px;
  right:10px;
  background:var(--amazon);
  padding:5px 8px;
  font-size:12px;
  font-weight:700;
  border-radius:6px;
}

/* 🔥 PRODUCT NAME – FINAL */
.product-card h3{
  font-size:14px;
  margin:12px 0;
  line-height:1.4;
  height:38px;
  overflow:hidden;

  color:var(--product-text-color, #000000) !important;
  font-weight:700 !important;
}

/* BUTTON */
.buy-btn{
  margin-top:auto;
  text-align:center;
  background:var(--amazon);
  color:#111;
  padding:12px;
  border-radius:10px;
  text-decoration:none;
  font-weight:700;
}
.buy-btn:hover{
  background:var(--flipkart);
  color:#fff;
}
</style>

<a data-encoded-tag-name="script" data-encoded-tag-value="JTBBY29uc3QlMjBBUElfVVJMJTNEJTIyaHR0cHMlM0ElMkYlMkZzY3JpcHQuZ29vZ2xlLmNvbSUyRm1hY3JvcyUyRnMlMkZBS2Z5Y2J5OElMUlhkVm9GNGExaTZXRHRvU0pUSGNnQVJ4d2hsTXNQN05oLVJEX2ZrSFBycndlYXdpbHdvSVhTSXJWc1N5UVFMQSUyRmV4ZWMlMjIlM0IlMEElMEFmZXRjaChBUElfVVJMKSUwQS50aGVuKHJlcyUzRCUzRXJlcy5qc29uKCkpJTBBLnRoZW4oZGF0YSUzRCUzRSU3QiUwQSUyMCUyMGNvbnN0JTIwJTdCc2V0dGluZ3MlMkNwcm9kdWN0cyU3RCUzRGRhdGElM0IlMEElMjAlMjBjb25zdCUyMGFwcCUzRGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKCUyMmFwcCUyMiklM0IlMEElMEElMjAlMjAlMkYqJTIwJUYwJTlGJTk0JUE1JTIwQ09OTkVDVCUyMFNIRUVUJTIwJUUyJTg2JTkyJTIwQ1NTJTIwKiUyRiUwQSUyMCUyMGRvY3VtZW50LmRvY3VtZW50RWxlbWVudC5zdHlsZS5zZXRQcm9wZXJ0eSglMEElMjAlMjAlMjAlMjAnLS1wcm9kdWN0LXRleHQtY29sb3InJTJDJTBBJTIwJTIwJTIwJTIwc2V0dGluZ3MuVEVYVF9DT0xPUiUyMCU3QyU3QyUyMCclMjMwMDAwMDAnJTBBJTIwJTIwKSUzQiUwQSUwQSUyMCUyMGNvbnN0JTIwY2F0ZWdvcmllcyUzRCU1Qi4uLm5ldyUyMFNldChwcm9kdWN0cy5tYXAocCUzRCUzRXAuQ0FURUdPUlkpKSU1RCUzQiUwQSUwQSUyMCUyMGFwcC5pbm5lckhUTUwlM0QlNjAlMEElMjAlMjAlMjAlMjAlM0NkaXYlMjBjbGFzcyUzRCUyMm9mZmVyLXdyYXBwZXIlMjIlM0UlMEElMjAlMjAlMjAlMjAlMjAlMjAlM0NkaXYlMjBjbGFzcyUzRCUyMm9mZmVyLXRpdGxlJTIyJTNFJTI0JTdCc2V0dGluZ3MuU0lURV9USVRMRSU3RCUzQyUyRmRpdiUzRSUwQSUyMCUyMCUyMCUyMCUyMCUyMCUzQ2RpdiUyMGNsYXNzJTNEJTIyY2F0LWJhciUyMiUzRSUwQSUyMCUyMCUyMCUyMCUyMCUyMCUyMCUyMCUyNCU3QmNhdGVnb3JpZXMubWFwKGMlM0QlM0UlNjAlM0NidXR0b24lMjBjbGFzcyUzRCUyMmNhdC1idG4lMjIlMjBkYXRhLWNhdCUzRCUyMiUyNCU3QmMlN0QlMjIlM0UlMjQlN0JjJTdEJTNDJTJGYnV0dG9uJTNFJTYwKS5qb2luKCUyMiUyMiklN0QlMEElMjAlMjAlMjAlMjAlMjAlMjAlM0MlMkZkaXYlM0UlMEElMjAlMjAlMjAlMjAlMjAlMjAlM0NkaXYlMjBjbGFzcyUzRCUyMnByb2R1Y3QtZ3JpZCUyMiUyMGlkJTNEJTIyZ3JpZCUyMiUzRSUzQyUyRmRpdiUzRSUwQSUyMCUyMCUyMCUyMCUzQyUyRmRpdiUzRSUwQSUyMCUyMCU2MCUzQiUwQSUwQSUyMCUyMGNvbnN0JTIwZ3JpZCUzRGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKCUyMmdyaWQlMjIpJTNCJTBBJTBBJTIwJTIwZnVuY3Rpb24lMjByZW5kZXIoY2F0KSU3QiUwQSUyMCUyMCUyMCUyMGdyaWQuaW5uZXJIVE1MJTNEJTIyJTIyJTNCJTBBJTIwJTIwJTIwJTIwcHJvZHVjdHMuZmlsdGVyKHAlM0QlM0VwLkNBVEVHT1JZJTNEJTNEJTNEY2F0KS5mb3JFYWNoKHAlM0QlM0UlN0IlMEElMjAlMjAlMjAlMjAlMjAlMjBncmlkLmlubmVySFRNTCUyQiUzRCU2MCUwQSUyMCUyMCUyMCUyMCUyMCUyMCUyMCUyMCUzQ2RpdiUyMGNsYXNzJTNEJTIycHJvZHVjdC1jYXJkJTIyJTNFJTBBJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTI0JTdCcC5UT1AlM0QlM0QlM0QlMjJZRVMlMjIlMjAlM0YlMjAlNjAlM0NkaXYlMjBjbGFzcyUzRCUyMmJhZGdlLXRvcCUyMiUzRSUyNCU3QnNldHRpbmdzLlRPUF9CQURHRV9URVhUJTdEJTNDJTJGZGl2JTNFJTYwJTNBJTIyJTIyJTdEJTBBJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTNDZGl2JTIwY2xhc3MlM0QlMjJiYWRnZS1vZmYlMjIlM0UlMjQlN0JwLkRJU0NPVU5UJTdEJTI1JTIwT0ZGJTNDJTJGZGl2JTNFJTBBJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTIwJTNDaW1nJTIwc3JjJTNEJTIyJTI0JTdCcC5JTUFHRSU3RCUyMiUzRSUwQSUyMCUyMCUyMCUyMCUyMCUyMCUyMCUyMCUyMCUyMCUzQ2gzJTNFJTI0JTdCcC5OQU1FJTdEJTNDJTJGaDMlM0UlMEElMjAlMjAlMjAlMjAlMjAlMjAlMjAlMjAlMjAlMjAlM0NhJTIwY2xhc3MlM0QlMjJidXktYnRuJTIyJTIwaHJlZiUzRCUyMiUyNCU3QnAuTElOSyU3RCUyMiUyMHRhcmdldCUzRCUyMl9ibGFuayUyMiUzRVZpZXclMjBvbiUyMEFtYXpvbiUzQyUyRmElM0UlMEElMjAlMjAlMjAlMjAlMjAlMjAlMjAlMjAlM0MlMkZkaXYlM0UlMEElMjAlMjAlMjAlMjAlMjAlMjAlNjAlM0IlMEElMjAlMjAlMjAlMjAlN0QpJTNCJTBBJTIwJTIwJTdEJTBBJTBBJTIwJTIwZG9jdW1lbnQucXVlcnlTZWxlY3RvckFsbCglMjIuY2F0LWJ0biUyMikuZm9yRWFjaChidG4lM0QlM0UlN0IlMEElMjAlMjAlMjAlMjBidG4ub25jbGljayUzRCgpJTNEJTNFJTdCJTBBJTIwJTIwJTIwJTIwJTIwJTIwZG9jdW1lbnQucXVlcnlTZWxlY3RvckFsbCglMjIuY2F0LWJ0biUyMikuZm9yRWFjaChiJTNEJTNFYi5jbGFzc0xpc3QucmVtb3ZlKCUyMmFjdGl2ZSUyMikpJTNCJTBBJTIwJTIwJTIwJTIwJTIwJTIwYnRuLmNsYXNzTGlzdC5hZGQoJTIyYWN0aXZlJTIyKSUzQiUwQSUyMCUyMCUyMCUyMCUyMCUyMHJlbmRlcihidG4uZGF0YXNldC5jYXQpJTNCJTBBJTIwJTIwJTIwJTIwJTdEJTBBJTIwJTIwJTdEKSUzQiUwQSUwQSUyMCUyMGRvY3VtZW50LnF1ZXJ5U2VsZWN0b3IoJTIyLmNhdC1idG4lMjIpLmNsaWNrKCklM0IlMEElN0QpJTNCJTBB"></a> 
