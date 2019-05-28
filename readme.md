
TODO: pretty, young-hearts-of-summer gif of humans & computer usage

# CHIRP NOTATION

TODO: version 1

TODO: "one thousand songs in your pocket" -- sell a lifestyle!

## OVERVIEW

TODO

### EASY TO READ

TODO: vertical
TODO: numeric
TODO: can be written as stringed-instrument tablature
TODO: consistent operators that build on each other

### EASY TO WRITE

TODO: "loose"
TODO: works well on normal college-ruled paper
TODO: plain-text!

### EASY TO EXPRESS

TODO: separate by "melodic-chain" rather than by pitch
TODO:  ie group in as many tonal sections as you want
TODO: encourages notes! great for capturing the *spirit* of the work
TODO: coming soon: formal way of expressing timbre, and evolution thereof
TODO: multiple ways to say things
TODO:   eg duration as lines or operators
TODO:   eg anchored/unanchored melodies
TODO:   eg numerical or symbolic chords
TODO: operators! eg repetition

### EASY TO TRANSPOSE

TODO: relative, rather than absolute
TODO:  good for "rebasing" to different orchestral instruments
TODO: multiply / divide by 10

### EASY TO COMPUTE

TODO: obviously

### EASY TO EXPERIMENT

TODO: want to change your number base? no problem! you just got a n-note chromatic scale
TODO: want to express microtones? no problem! just use decimals or fractions

### EASY TO EXCEL

TODO: easier to learn advanced theory
TODO:   numbers make the relations between math & music VERY clear
TODO: the notation attempts to bring music back closer to physics & math

## TUTORIAL

TODO

## FURTHER READING

- [Dozenal / Duodecimal / Base-12](https://en.wikipedia.org/wiki/Duodecimal)
- [Music & Mathematics](https://en.wikipedia.org/wiki/Music_and_mathematics)
- [Harmony Explained: Progress Towards A Scientific Theory of Music](https://arxiv.org/html/1202.4212v2)

## NOTES

TODO: other possible names: croak, grunt, squawk, wheeze, mumble, growl, moo, ribbit

TODO: lots of pictures!

TODO: find a better way of expressing "complex chords"
TODO:   add symbols to a root note!
TODO:     eg `0-*¨` could be a major-7 chord
TODO:     eg `0_.-=+°¨^` could be all the notes of the major key
TODO:     prefix/suffix for negative/positive harmony
TODO:     pipe represents a new octave, so `0|.` adds the major second from the next octave
TODO:     ascending height options : _,.-~¬«=×*+°'^¨¯|
TODO:     ascii options: ¸ ! " # $ % & ' () * + , - . / : ; < = > ? @ [ \ ] ^ _ ` { | } ~ ¡ ¢ £ ¤ ¥ ¦ § ¨ © ª « ¬ ® ¯ ° ± ² ³ ´ µ ¶ · ¸ ¹ º » ¼ ½ ¾ ¿ × Ø – — ‘ ’ ‚ “ ” „ † ‡ • … 

    0 1 2 3 4 5 6 7 8 9 Ɛ ? 10 10 10 11 ...
    _ , . ¬ ~ = + * ° ' ¨ ^ ¯  |  _  ,  ...
    
TODO: what's the best way to communicate duration? and glissando?
TODO:   i don't feel like all these weird bars are doing the job well
TODO:     i like the idea of making multipliers of beat (in Hz) that change the duration by different multiples

    ... 0.3 0.46 0.6 0.9 1.0 1.6 2.0 3.0 4.0 ... 8.0 ...
    ...  «   <\   <   \   •   /   >   />  »  ... >>> ...
    
    'til next-note end-of-measure end-of-piece
         :         ::             :::

    'til next-note end-of-measure end-of-piece (legato/glissando)
         ;         ;;             ;;;
    
    [•n] repeat every beat n-times
    [<n] repeat every half-beat n-times
    ...
    {•n} repeat every measure n-times
    {>n} repeat every other measure n-times
    ...

TODO: it's probably best to optimize for *paper & web* rather than *paper & plain-text*

TODO: columns are "dimensions"
TODO:   time column has header describing measure-length
TODO:     make sure it's MEASURE length and not beat length
TODO:       it should have its own column in case you need to vary it
TODO:   pitch column has header describing pitch-basis (0 freq)
TODO:   feel free to add additional things like vibrato and envelope modulation
TODO:     for example, you may want to group intensity columns with different hands

TODO: OOOOOOO you can make a tone-group for each string (eg guitar) and you have tabs! just put n (eg 6) tone-groups next to each other

BUG: too many ways to express things...

    ===============================================================================================
    ¦ GLOBAL              ¦  TONE-GROUP   ¦  TONE-GROUP ¦  TONE-GROUP        ¦  TONE-GROUP        ¦
    ===============================================================================================
    ¦ time meas beat vibr ¦  pitch intens ¦  pitch      ¦  pitch wave        ¦  pitch wave        ¦
    ¦      .5Hz 2Hz  5Hz  ¦  440Hz pp     ¦  440Hz      ¦  440Hz sgn(cos(x)) ¦  440Hz sgn(sin(x)) ¦
    ===============================================================================================
    ¦ 0.0            5Hz  ¦  0_           ¦        0~   ¦  • 14_             ¦  >                 ¦
    ¦ 0.16           |    ¦  |            ¦        |    ¦                    ¦                    ¦
    ¦ 0.3            |    ¦  |            ¦     0.      ¦  • 12_             ¦                    ¦
    ¦ 0.46           |    ¦  |=           ¦     |       ¦                    ¦                    ¦
    ¦ 0.6            |    ¦  |            ¦  0_         ¦  • 10_             ¦  • 20_             ¦
    ¦ 0.86           |    ¦  |            ¦  |          ¦                    ¦                    ¦
    ¦ 0.9            |    ¦  |*           ¦     0.      ¦  • 12_             ¦  • 22_             ¦
    ¦ 0.Ɛ6           |    ¦  |            ¦     |       ¦                    ¦                    ¦
    -----------------------------------------------------------------------------------------------
    ¦ 1.0            7Hz  ¦  0_=*         ¦        0~   ¦  • 4|_             ¦  />                ¦
    ¦ 1.3                 ¦  |            ¦        0~   ¦  • 4|_             ¦                    ¦
    ¦ 1.6                 ¦  |            ¦        0~   ¦  > 4|_             ¦                    ¦
    ¦ 1.9                 ¦               ¦        |    ¦                    ¦ :: 0= 0*           ¦
    -----------------------------------------------------------------------------------------------
    ¦ 2.0                 ¦ ,0=*          ¦     0.      ¦  • 2¯              ¦  />                ¦
    ¦ 2.3                 ¦  |            ¦     0.      ¦  • 2¯              ¦                    ¦
    ¦ 2.6                 ¦  |            ¦  :: 0.      ¦  > 2¯              ¦                    ¦
    ¦ 2.9                 ¦               ¦             ¦                    ¦  • 0= 0*           ¦
    -----------------------------------------------------------------------------------------------
