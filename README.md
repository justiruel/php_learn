# php_learn

## Convert array to json
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
