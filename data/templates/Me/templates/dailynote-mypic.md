.action{ $ppath := nospace (cat "https://cdn.jsdelivr.net/gh/lanedu/SiYuan@main/pic/pic" ((randInt 1 234) | toString) ".jpg")}

.action{$after := (div ((toDate "2006-01-02" "2021-11-05").Sub now).Hours 24)}

.action{$dayleft := (div ((toDate "2006-01-02" "2022-01-01").Sub now).Hours 24)}

.action{$week := add (mod (div ((toDate "2006-01-02" "2050-03-13").Sub now).Hours 24) 7) 1}

![image.png](.action{$ppath})

### π  ζ©η‘ζ©θ΅· 


> π εε»ΊζΆι΄οΌ.action{now | date "2006-01-02 15:04"} .action{last (slice (list "ζζε­" "ζζδΊ" "ζζε" "ζζδΈ" "ζζδΊ" "ζζδΈ" "ζζε€©") 0 $week )}

