# PinView
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Pinterest Clone</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
    margin:0;
    font-family:Arial, sans-serif;
    background:#111;
    color:white;
}

/* HEADER */
header{
    position:sticky;
    top:0;
    background:#111;
    padding:10px;
    display:flex;
    align-items:center;
    gap:10px;
    z-index:100;
}
.logo{
    font-size:22px;
    font-weight:bold;
    color:#e60023;
}
.search{
    flex:1;
    padding:10px;
    border-radius:25px;
    border:none;
    outline:none;
    background:#222;
    color:white;
}

/* GRID */
.grid{
    column-count:4;
    column-gap:12px;
    padding:12px;
}
@media(max-width:900px){ .grid{column-count:3;} }
@media(max-width:600px){ .grid{column-count:2;} }
@media(max-width:400px){ .grid{column-count:1;} }

.pin{
    background:#222;
    margin-bottom:12px;
    border-radius:16px;
    overflow:hidden;
    break-inside:avoid;
    position:relative;
    cursor:pointer;
}
.pin img{
    width:100%;
    display:block;
}

/* HOVER SAVE */
.save{
    position:absolute;
    top:10px;
    right:10px;
    background:#e60023;
    padding:6px 12px;
    border-radius:20px;
    font-size:14px;
    display:none;
}
.pin:hover .save{
    display:block;
}
</style>
</head>

<body>

<header>
    <div class="logo">Pinterest</div>
    <input class="search" placeholder="Search ideas">
</header>

<div class="grid">
    <div class="pin">
        <img src="https://picsum.photos/300/500?1">
        <div class="save">Save</div>
    </div>
    <div class="pin">
        <img src="https://picsum.photos/300/400?2">
        <div class="save">Save</div>
    </div>
    <div class="pin">
        <img src="https://picsum.photos/300/600?3">
        <div class="save">Save</div>
    </div>
    <div class="pin">
        <img src="https://picsum.photos/300/350?4">
        <div class="save">Save</div>
    </div>
    <div class="pin">
        <img src="https://picsum.photos/300/550?5">
        <div class="save">Save</div>
    </div>
    <div class="pin">
        <img src="https://picsum.photos/300/420?6">
        <div class="save">Save</div>
    </div>
</div>

</body>
</html>
