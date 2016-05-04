# ZCP-A3-Exile

Install info @ [ZCP @ Exile forums](http://www.exilemod.com/topic/12116-release-official-zcp-zupas-capture-points/)



### BE filters

These are kicks based on what i encountered:

on the line of 'isPlayer' add
```
!="if (isPlayer _this) then {}"
```

on the line of 'units' add
```
!="if (count units group _this>1) then"
```

Changes in 2.1

* Amount of starting AI is now defined per mission instead of global.
* You can now pass an array of bases to the basetype of a cappoint to randomly choose from.
* Code cleanup.
* Fixed cappoint not being capable ( problem with non private variables ).
* Allow muliple rewards for 1 mission.
* Option to deploy smokescreen per missions after finishing it.
* Option to pass list/array of basesfiles per mission (Instead of only Random or 1 basefile).
* No longer need to define baseType in the Cappoints array. It will auto determine it from the cappbases array.
* Add m3e export base support
* Option to disable damage when bombing is happening on map and build objects ( people and vehicles still die ).
* Added minimum distance check to Exile buildables