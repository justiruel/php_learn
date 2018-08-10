# php_learn

# Convert array to json
```
http://www.dyn-web.com/tutorials/php-js/json/multidim-arrays.php
```
## contoh
```
$food_groups = array(
    'meat' => array(),
    'vegetables' => array(
        'leafy' => array('collard greens', 'kale', 'chard', 'spinach', 'lettuce'),
        'root' => array('radish', 'turnip', 'potato', 'beet'),
        'other' => array('brocolli', 'green beans', 'corn', 'tomatoes')
    ),
    'grains' => array('bread', 'rice', 'oatmeal'),
    'legumes' => array('kidney beans', 'lentils', 'split peas'),
    'fruits' => array('apple', 'raspberry', 'pear', 'banana'),
    'sweets' => array('cookies', 'brownies', 'cake', 'pie'),
);
```
## menjadi
```
{
    "meat":[],
    "vegetables":{
        "leafy":["collard greens","kale","chard","spinach","lettuce"],
        "root":["radish","turnip","potato","beet"],
        "other":["brocolli","green beans","corn","tomatoes"]
    },
    "grains":["bread","rice","oatmeal"],
    "legumes":["kidney beans","lentils","split peas"],
    "fruits":["apple","raspberry","pear","banana"],
    "sweets":["cookies","brownies","cake","pie"]
}
```
<b>vegetables kenapa jadi Jsonobject? karena ada associative array didalamnya " 'leafy' => array()  "</b><br/>
<b>leafy kenapa jadi JsonArray? karena tidak ada associative array didalamnya </b>

cat. associative array adalah array yang index nya berupa string


# Convert stdClass to array
```
$output = json_decode(json_encode($stdclass_variable), true); //When TRUE, returned objects will be converted into associative arrays.
```

# json_decode($array,true)
param 'true' untuk membuat agar array di convert ke associative array (array yang index nya string)

# json_encode
convert stdObject / array ke JSON String, contoh:
```
$data = ["nama"=>"irul","alamat"=>"malang","web"=>"http://tafsirul.web.id"];
echo json_encode($data);
```
hasilnya berupa string jadi jika ingin digunakan sebagai string tidak perlu di stringify:
```
{"nama":"irul","alamat":"malang","web":"http:\/\/tafsirul.web.id"}
```



