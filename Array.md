```
<?php
function prefix($nama, $umur){
    return "mas ".$nama." umur ".$umur;
}

$nama = array("joko","joni","ridwan");
$umur = array(21,30,40);

echo "<pre/>";
$a = array_map(null,$nama,$umur);
print_r($a);

$b = array_map("prefix",$nama,$umur);
print_r($b);

$array_keys = array_keys($nama);
print_r($array_keys);

echo $sum_umur = array_sum($umur)."<br/>";
echo $average_umur = array_sum($umur) / count($umur)."<br/>";
echo 7/8; echo "<br/>";
echo round(7/8); echo "<br/>";
echo ceil(7/8); echo "<br/>";
echo floor(7/8); echo "<br/>";

//collection group by




?>
```
