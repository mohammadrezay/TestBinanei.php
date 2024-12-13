# TestBinanei.php
https://quera.org/problemset/2659?tab=description
<?php
$n = (int)readline("Enter a number: ");
$GozashteShode = (string)readline("Enter a string: ");
$NeveshteShode = (string)readline("Enter a string: ");
$G = preg_split('//u', $GozashteShode, null, PREG_SPLIT_NO_EMPTY);
$N = preg_split('//u', $NeveshteShode, null, PREG_SPLIT_NO_EMPTY);
$eshtebah = 0;
for($i = 0; $i <= $n; $i++){
	if($N[$i] !== $G[$i]){
		$eshtebah += 1;
	}
}
echo $eshtebah ;
