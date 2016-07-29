Tafseer As-Sa'di (English)
==========================


                                       ‫بسم الله الرَّحْمَنِ الرَّحِيمِ


We are taking an initiative to compile authentic translation of _Taysir al-Karim ar-Rahman fee Tafsir al-Quran_ also known as Tafseer As-Sa'di by Sheikh Abd ar-Rahman ibn Nasir as-Sa'di at-Tamimi (d. 1956)

Introduction to Tafsir As-Sa'di
-------------------------------

Tafsir As-Sa'di is a straightforward, easy to read, easy to understand explanation of the meaning of Qur'anic Ayat and statements. In addition to the simplicity of Ibn Sa'di's writing, it is also articulate and eloquent.

Consequently, for those newly acquainted with Tafsir and those new to Islam, this Tafsir provides an uncomplicated, deep and insightful comprehension into the meaning and explanation of the Qur'an.

The uniqueness of this Tafsir is in the style the Shaikh used to explain the Ayat in a way that it is similar to everyday writing, without listing the various prophetic sayings or statements of the scholars of Tafsir, which Shaikh Ibn Sa'di used as a basis of his Tafsir.

Files
-----

We want to support as many platforms as possible so we do not want to make a restriction of certain format (e.g, SQL). We have come to conclusion that we are going to have 1-file rule that means each ayah will be in it's own file. 

File naming will be `<Surah>-<Ayah>.txt`. For example, tafseer of Surah Ash-Shura Ayah 11 will be in file called `42-11.txt` under directory `42`.

Format
------

While writing tafseer you would also follow guidelines that will make it easy to read. Parsers will be written to follow these guidelines as well.

There are following types of text within tafseer:

 - 1. General text
 - 2. Text from ayah (e.g, if you are doing tafseer of `42:11`, the text from `42:11`)
 - 3. Text from another ayah (e.g, if the tafseer contains reference of another ayah from Quran)
 - 4. Hadeeth text
 - 5. Other texts 

When writing tafseer, you choose rule by `:RULE_NUMBER{TEXT}`. Except for rule #1 that you do not need to specify.

For example a text
```
This is general text where as :2{text from ayah} is rule 2 and :3{text from another ayah} is rule three and so on.
```
Our parsers will then transform this text as

This is general text where as **text from ayah** is rule 2 and __text from another ayah__ is rule three and so on.

The parsers will be linient and rules will be easily changeable, for example, someone can write parser to show `text from ayah` as blue text. This is why we have made our own rules.

---

May Allah make it easy for us to finish this and help our ummah and deen. May Allah accept it from us enter us in to jannat-ul firdous with His Mercy. Aameen
