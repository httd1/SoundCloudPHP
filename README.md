# SoundCloudPHP
Class to download from SondCloud

```php

include 'SoundCloudPHP.php';

try {

	$sc = new SoundCloudPHP ();
	$data_music = $sc->getMusicInfo ('https://soundcloud.com/vintageculturemusic/vintage-culture-x-bye-bad-new-life-2021-bondinho-pao-de-acucar');
	
	echo 'URL download '.$sc->getMusic ($data_music ['media']['transcodings'][1]['url']);

}catch (Exception $e){
	echo $e->getMessage ();
}

```
