
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


## MORE NOTES

TODO: Start from scratch! We need a simple system.
TODO: We need a notation of (1) pitch, (2) duration, (3) amplitude, and (4) repetition. That's it. Everything else is metadata.

TODO: I kind of like the idea of separating rhythm from pitch.

TODO: Pitches operate in a "pitch context" and durations operate in a "duration context".
TODO: Duration contexts are in Hz, which determine the length of each beat.

TODO: Each rhythm group represents a beat.

    In traditional music terms:
    ---------------------------
    ''         | two half-notes
    '''        | triplets
    ''''       | four quarter-notes
    '.'.       | two quarter-notes with rests afterward
    '-'-       | two half-notes
    '-''       | half-note then two quarter notes
    '...       | quarter-note
    '|=        | two whole notes (continued into the next bar)
    '|=|=      | three whole notes (continued into the next bars)
    '|=.       | a whole-note and a half
    .--'|=...  | a half-note starting on the fourth beat of the measure
    ['.]...    | an eight-note
    ....|*4    | repeat beat 4 times
    .|.|*3     | repeat two beats 3 times
    '..^..'.'. | accent
    
    
TODO: Rhythm groups are applied to pitches.

    '-''      0 2 4 
    '...      2
    '-.-.-.-  2
    ''''''''  0 2 4 5 7 9 B

TODO: Columns can represent parallel parts!

    | '-''      0 2 4          | '-......  2
    | '...      2              | ''''''''  0 2 4 5 7 9 B
    | '-......  2              | '-''      0     2   4
    | ''''''''  0 2 4 5 7 9 B  | ...[.']               2
    
TODO: Tricky/fast parts can be broken out with brackets.

    '''.
    '    0
         0
    '.'' 0 2 4
    
TODO: Display for writing vs. reading needn't be the same. 
TODO: To perform, it may be best to go vertical (receipt paper for physical and auto-scroller for screen). 
TODO: Also add unique colors to each note for easier scanning.
BUG: The headers need work.

    | 2Hz       | 2Hz
    | C:A%438Hz | C:A%438Hz
    | 60dB      | 60dB
    |           |
    | '-''      | [''''].'.'''
    |           |
    | 0         | 0  2  4  5
    |           |       7
    | 2         |       9
    | 4         | B    |0 
    |           |
    | '         | .
    |           |
    | 0         |

TODO: Pitch headers.
BUG: Hard to parse! Make atoms with prefixes that can be combined in any order.
BUG: These suck.

    | *:C               | Key of C in chromatic notation
    | *:C:%A438Hz       | Key of C where A is 438Hz in chromatic notation
    | *:C:eq            | Key of C in equal temperament in chromatic notation
    | *:C:%A438Hz:just  | Key of C where A is 438Hz in just intonation and chromatic notation
    | #:E4              | E4 guitar string in tab notation
    | ^                 | Automation and effects levels
    | !                 | Percussion.
    | _                 | No pitch

TODO: Chords!

    '''''
    0469
    0_~+'
    0M7
    C#E#F#B#
    CbEbFbBb

TODO: Example: syncopation and repetition.

    '..'..'..'..'..'   0 0 0 0 0 0
    '..'..'..'..'..'   [0]::6
    '..'..'..'..'..'   [0]::
    '..'..'..'..'..'   |[0|]::

TODO: Split rhythms.

    ''.' [' 0 | '... 4] 6 9

TODO: Accents/stacatto go in the rhythm sections, while expressions like legato and glissando go with the pitch.

    | %:0       | trill
    | &:0M      | roll
    | (0 4 6)   | glide/slide
    | 0 $1      | bend
    | 0 /:1     | bend
    | /:1 \:0   | unbend
    | 0 <:1     | hammer on
    | <:1 >:0   | hammer off


TODO: Measures and parts.
BUG: Change this to double-colon/double-pipe syntax.

    | ''.' '.'' .... ....  | '... '... .... ....
    | [0]::                | 0 0

    | ''.' '.'' .... .... [0]:: | '... '... .... .... 0 0

    | ''.' '.'' .... .... [0]::
    | '... '... .... .... 0 0

    | ''.' '.'' .... .... 
      [0]::
    | '... '... .... .... 
      0 
      0

TODO: Tracks need to be able to have names that can be mixed for bus-like combinations.

TODO: Instruments and effects via functions! 
TODO: Also need note-generators functions, etc.
TODO: Functions should be allowed to applied to pretty much anything.

    (asdr 1 1 1 1) sine [' 1]

TODO: If we make this a functional queue language, then the rhythms are just function sugar and the pipes switch queue.
TODO: Actually, it would probably work better if all the rhythms and pitches were just mixed together however and the "song" function figured out how to mash them.
TODO:   This makes it so that we can use `' ' ' ' 0 0 0 0` and `' 0 | ' 0 | ' 0 | ' 0` interchangably.
TODO:   Therefore a "song" would be a list of rhythms, pitches, and instrument/sequence markers that get folded together.

    '''' ;; a function that takes four "events" as inputs and produces a sequence
    '''' ;; ACTUALLY just a rhythm value
    A#   ;; a value as pitch as note
    024  ;; a value as pitch as chord
    [0]  ;; a value as queue of pitch as note
    [' 0 | .' 1] 
    

TODO: Consider making the pipe mean "and-then" and the colon mean "concurrently".
TODO: Single pipe would mean next-beat for same instrument, and double-colon would mean concurrently with next instrument. Double pipe for next-beat for all instruments.
TODO: I really like this!

    || [' 0 : .' 1] | '' 2 2 
    :: ' 0          | '' 4 4
    || ' 2          | '' 2 2 
    :: ' 0          | '' 4 4
