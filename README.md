
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        span {
            color:red;
        }
    </style>
</head>
<body>
    <?php
     $a=array(
        array(5,2,9,5,7,7,4,4),
        array(6,4,8,7,6,7,3,8),
        array(3,5,7,1,5,6,4,5),
        array(0,8,2,3,6,4,3,7),
        array(0,8,6,4,7,4,3,2),        
     );
     /*$min=$a[0][0]; $max=$a[0][0];
     for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){
            echo $a[$i][$j]." ";
               if($min>$a[$i][$j]){
                   $min=$a[$i][$j];
               }   
               if($max<$a[$i][$j]){
                $max=$a[$i][$j];
            } 
        }
        echo "---min:".$min." max:".$max;
        if($i+1<count($a)){
        $min=$a[$i+1][0];
        $max=$a[$i+1][0];
        }
        echo "<br>";
     }*/
     /*$y=0;
     for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){
            $y=$y+$a[$i][$j];
            echo $a[$i][$j]." ";
        }
        echo "--".$y;
        $y=0;
        echo "<br>";
     }*/
     /*$s=0;
     for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){
            if($a[$i][$j]%2==1){
                echo "<span>".$a[$i][$j]."</span> ";
                $s=$s+$a[$i][$j];
            }else {
            echo $a[$i][$j]." ";
            }
        }
        echo "-->".$s;
        $s=0;
        echo "<br>";
     }
     echo $s;*/
     /*$s=0;
     for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){
            if($a[$i][$j]%2==0){
                echo "<span>".$a[$i][$j]."</span> ";
                $s++;
            }else {
            echo $a[$i][$j]." ";
            }
        }
        echo "-->".$s;
        $s=0;
        echo "<br>";
     }
     echo $s;*/
     /*$s=0;
     for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){            
            if($j==0){
                echo $a[$i][$j]." ";
                continue;
            }
            if($a[$i][$j]<$a[$i][$j-1]){
                echo "<span>".$a[$i][$j]."</span> ";
            } else {
                echo $a[$i][$j]." ";
            }
        }
        echo "<br>";
     }  */
     /*$s=0;
     for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){            
            if($j==0 || $j==count($a[$i])-1){
                echo $a[$i][$j]." ";
                continue;
            }
            if($a[$i][$j]<$a[$i][$j-1] && $a[$i][$j]<$a[$i][$j+1]){
                echo "<span>".$a[$i][$j]."</span> ";
            } else {
                echo $a[$i][$j]." ";
            }
        }
        echo "<br>";
     } */
    /* for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){            
            if($i==0 || $i==count($a)-1){
                echo $a[$i][$j]." ";
                continue;
            }
            if($a[$i][$j]<$a[$i-1][$j] && $a[$i][$j]<$a[$i+1][$j]){
                echo "<span>".$a[$i][$j]."</span> ";
            } else {
                echo $a[$i][$j]." ";
            }
        }
        echo "<br>";
     } */
     /*for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){  
            if($i==0 ||$j==0){
                echo $a[$i][$j]." ";
                continue;
            }
            if($a[$i][$j]<$a[$i-1][$j-1]){
                echo "<span>".$a[$i][$j]."</span> ";
            } else {
                echo $a[$i][$j]." ";
            }
            #echo $a[$i][$j]." ";
        }
        echo "<br>";
     }*/
     /*for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){  
            if($i==0 ||$j==0 ||$i==count($a)-1 ||$j==count($a[$i])-1){
                echo $a[$i][$j]." ";
                continue;
            }
            if($a[$i][$j]<$a[$i-1][$j-1] && $a[$i][$j]<$a[$i+1][$j+1]){
                echo "<span>".$a[$i][$j]."</span> ";
            } else {
                echo $a[$i][$j]." ";
            }
        }
        echo "<br>";
     }*/
     for($i=0;$i<count($a);$i++){
        for($j=0;$j<count($a[$i]);$j++){  
            if($i==0 ||$j==0 ||$i==count($a)-1 ||$j==count($a[$i])-1){
                echo $a[$i][$j]." ";
                continue;
            }
            if($a[$i][$j]<$a[$i-1][$j+1] && $a[$i][$j]<$a[$i+1][$j-1]){
                echo "<span>".$a[$i][$j]."</span> ";
            } else {
                echo $a[$i][$j]." ";
            }
        }
        echo "<br>";
     }
    ?>
</body>
</html>
