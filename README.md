# date-formats
A running list of date formats based on language/library for reference.

# Contents
- [.Net](#net)
- [Ruby](#ruby)
- [JS](#js)
 - [Moment](#moment)




# [.Net](#net) 
([source](https://msdn.microsoft.com/en-us/library/8kb3ddd4(v=vs.110).aspx))

<div class="contentTableWrapper"><table responsive="true" summary="table"><tbody><tr responsive="true"><th scope="col"><p>Format specifier</p></th><th scope="col"><p>Description</p></th><th scope="col"><p>Examples</p></th></tr><tr><td data-th="Format specifier"><p>"d"</p></td><td data-th="Description"><p>The day of the month, from 1 through 31. </p><p>More information: <a href="#dSpecifier">The "d" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-01T13:45:30 -&gt; 1</p><p>2009-06-15T13:45:30 -&gt; 15</p></td></tr><tr><td data-th="Format specifier"><p>"dd"</p></td><td data-th="Description"><p>The day of the month, from 01 through 31.</p><p>More information: <a href="#ddSpecifier">The "dd" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-01T13:45:30 -&gt; 01</p><p>2009-06-15T13:45:30 -&gt; 15</p></td></tr><tr><td data-th="Format specifier"><p>"ddd"</p></td><td data-th="Description"><p>The abbreviated name of the day of the week.</p><p>More information: <a href="#dddSpecifier">The "ddd" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; Mon (en-US)</p><p>2009-06-15T13:45:30 -&gt; Пн (ru-RU)</p><p>2009-06-15T13:45:30 -&gt; lun. (fr-FR)</p></td></tr><tr><td data-th="Format specifier"><p>"dddd"</p></td><td data-th="Description"><p>The full name of the day of the week.</p><p>More information: <a href="#ddddSpecifier">The "dddd" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; Monday (en-US)</p><p>2009-06-15T13:45:30 -&gt; понедельник (ru-RU)</p><p>2009-06-15T13:45:30 -&gt; lundi (fr-FR)</p></td></tr><tr><td data-th="Format specifier"><p>"f"</p></td><td data-th="Description"><p>The tenths of a second in a date and time value.</p><p>More information: <a href="#fSpecifier">The "f" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6170000 -&gt; 6</p><p>2009-06-15T13:45:30.05 -&gt; 0 </p></td></tr><tr><td data-th="Format specifier"><p>"ff"</p></td><td data-th="Description"><p>The hundredths of a second in a date and time value.</p><p>More information: <a href="#ffSpecifier">The "ff" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6170000 -&gt; 61</p><p>2009-06-15T13:45:30.0050000 -&gt; 00</p></td></tr><tr><td data-th="Format specifier"><p>"fff"</p></td><td data-th="Description"><p>The milliseconds in a date and time value.</p><p>More information: <a href="#fffSpecifier">The "fff" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>6/15/2009 13:45:30.617 -&gt; 617</p><p>6/15/2009 13:45:30.0005 -&gt; 000</p></td></tr><tr><td data-th="Format specifier"><p>"ffff"</p></td><td data-th="Description"><p>The ten thousandths of a second in a date and time value.</p><p>More information: <a href="#ffffSpecifier">The "ffff" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6175000 -&gt; 6175</p><p>2009-06-15T13:45:30.0000500  -&gt; 0000</p></td></tr><tr><td data-th="Format specifier"><p>"fffff"</p></td><td data-th="Description"><p>The hundred thousandths of a second in a date and time value.</p><p>More information: <a href="#fffffSpecifier">The "fffff" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6175400 -&gt; 61754</p><p>6/15/2009 13:45:30.000005 -&gt; 00000</p></td></tr><tr><td data-th="Format specifier"><p>"ffffff"</p></td><td data-th="Description"><p>The millionths of a second in a date and time value.</p><p>More information: <a href="#ffffffSpecifier">The "ffffff" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6175420 -&gt; 617542</p><p>2009-06-15T13:45:30.0000005 -&gt; 000000</p></td></tr><tr><td data-th="Format specifier"><p>"fffffff"</p></td><td data-th="Description"><p>The ten millionths of a second in a date and time value.</p><p>More information: <a href="#fffffffSpecifier">The "fffffff" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6175425 -&gt; 6175425</p><p>2009-06-15T13:45:30.0001150 -&gt; 0001150</p></td></tr><tr><td data-th="Format specifier"><p>"F"</p></td><td data-th="Description"><p>If non-zero, the tenths of a second in a date and time value.</p><p>More information: <a href="#F_Specifier">The "F" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6170000 -&gt; 6</p><p>2009-06-15T13:45:30.0500000 -&gt; (no output)</p></td></tr><tr><td data-th="Format specifier"><p>"FF"</p></td><td data-th="Description"><p>If non-zero, the hundredths of a second in a date and time value.</p><p>More information: <a href="#FF_Specifier">The "FF" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6170000 -&gt; 61</p><p>2009-06-15T13:45:30.0050000 -&gt; (no output)</p></td></tr><tr><td data-th="Format specifier"><p>"FFF"</p></td><td data-th="Description"><p>If non-zero, the milliseconds in a date and time value.</p><p>More information: <a href="#FFF_Specifier">The "FFF" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6170000 -&gt; 617</p><p>2009-06-15T13:45:30.0005000 -&gt; (no output)</p></td></tr><tr><td data-th="Format specifier"><p>"FFFF"</p></td><td data-th="Description"><p>If non-zero, the ten thousandths of a second in a date and time value.</p><p>More information: <a href="#FFFF_Specifier">The "FFFF" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.5275000 -&gt; 5275</p><p>2009-06-15T13:45:30.0000500 -&gt; (no output)</p></td></tr><tr><td data-th="Format specifier"><p>"FFFFF"</p></td><td data-th="Description"><p>If non-zero, the hundred thousandths of a second in a date and time value.</p><p>More information: <a href="#FFFFF_Specifier">The "FFFFF" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6175400 -&gt; 61754</p><p>2009-06-15T13:45:30.0000050 -&gt; (no output)</p></td></tr><tr><td data-th="Format specifier"><p>"FFFFFF"</p></td><td data-th="Description"><p>If non-zero, the millionths of a second in a date and time value.</p><p>More information: <a href="#FFFFFF_Specifier">The "FFFFFF" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6175420 -&gt; 617542</p><p>2009-06-15T13:45:30.0000005 -&gt; (no output)</p></td></tr><tr><td data-th="Format specifier"><p>"FFFFFFF"</p></td><td data-th="Description"><p>If non-zero, the ten millionths of a second in a date and time value.</p><p>More information: <a href="#FFFFFFF_Specifier">The "FFFFFFF" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6175425 -&gt; 6175425</p><p>2009-06-15T13:45:30.0001150 -&gt; 000115</p></td></tr><tr><td data-th="Format specifier"><p>"g", "gg"</p></td><td data-th="Description"><p>The period or era.</p><p>More information: <a href="#gSpecifier">The "g" or "gg" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30.6170000 -&gt; A.D.</p></td></tr><tr><td data-th="Format specifier"><p>"h"</p></td><td data-th="Description"><p>The hour, using a 12-hour clock from 1 to 12.</p><p>More information: <a href="#hSpecifier">The "h" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T01:45:30 -&gt; 1</p><p>2009-06-15T13:45:30 -&gt; 1</p></td></tr><tr><td data-th="Format specifier"><p>"hh"</p></td><td data-th="Description"><p>The hour, using a 12-hour clock from 01 to 12.</p><p>More information: <a href="#hhSpecifier">The "hh" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T01:45:30 -&gt; 01</p><p>2009-06-15T13:45:30 -&gt; 01</p></td></tr><tr><td data-th="Format specifier"><p>"H"</p></td><td data-th="Description"><p>The hour, using a 24-hour clock from 0 to 23.</p><p>More information: <a href="#H_Specifier">The "H" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T01:45:30 -&gt; 1</p><p>2009-06-15T13:45:30 -&gt; 13</p></td></tr><tr><td data-th="Format specifier"><p>"HH"</p></td><td data-th="Description"><p>The hour, using a 24-hour clock from 00 to 23.</p><p>More information: <a href="#HH_Specifier">The "HH" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T01:45:30 -&gt; 01</p><p>2009-06-15T13:45:30 -&gt; 13</p></td></tr><tr><td data-th="Format specifier"><p>"K"</p></td><td data-th="Description"><p>Time zone information.</p><p>More information: <a href="#KSpecifier">The "K" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>With <a href="https://msdn.microsoft.com/en-us/library/system.datetime(v=vs.110).aspx">DateTime</a> values:</p><p>2009-06-15T13:45:30, Kind Unspecified -&gt; </p><p>2009-06-15T13:45:30, Kind Utc -&gt; Z</p><p>2009-06-15T13:45:30, Kind Local -&gt; -07:00 (depends on local computer settings)</p><p>With <a href="https://msdn.microsoft.com/en-us/library/system.datetimeoffset(v=vs.110).aspx">DateTimeOffset</a> values:</p><p>2009-06-15T01:45:30-07:00 --&gt; -07:00</p><p>2009-06-15T08:45:30+00:00 --&gt; +00:00</p></td></tr><tr><td data-th="Format specifier"><p>"m"</p></td><td data-th="Description"><p>The minute, from 0 through 59.</p><p>More information: <a href="#mSpecifier">The "m" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T01:09:30 -&gt; 9</p><p>2009-06-15T13:29:30 -&gt; 29</p></td></tr><tr><td data-th="Format specifier"><p>"mm"</p></td><td data-th="Description"><p>The minute, from 00 through 59.</p><p>More information: <a href="#mmSpecifier">The "mm" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T01:09:30 -&gt; 09</p><p>2009-06-15T01:45:30 -&gt; 45</p></td></tr><tr><td data-th="Format specifier"><p>"M"</p></td><td data-th="Description"><p>The month, from 1 through 12.</p><p>More information: <a href="#M_Specifier">The "M" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; 6</p></td></tr><tr><td data-th="Format specifier"><p>"MM"</p></td><td data-th="Description"><p>The month, from 01 through 12.</p><p>More information: <a href="#MM_Specifier">The "MM" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; 06</p></td></tr><tr><td data-th="Format specifier"><p>"MMM"</p></td><td data-th="Description"><p>The abbreviated name of the month. </p><p>More information: <a href="#MMM_Specifier">The "MMM" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; Jun (en-US)</p><p>2009-06-15T13:45:30 -&gt; juin (fr-FR)</p><p>2009-06-15T13:45:30 -&gt; Jun (zu-ZA)</p></td></tr><tr><td data-th="Format specifier"><p>"MMMM"</p></td><td data-th="Description"><p>The full name of the month.</p><p>More information: <a href="#MMMM_Specifier">The "MMMM" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; June (en-US)</p><p>2009-06-15T13:45:30 -&gt; juni (da-DK)</p><p>2009-06-15T13:45:30 -&gt; uJuni (zu-ZA)</p></td></tr><tr><td data-th="Format specifier"><p>"s"</p></td><td data-th="Description"><p>The second, from 0 through 59.</p><p>More information: <a href="#sSpecifier">The "s" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:09 -&gt; 9</p></td></tr><tr><td data-th="Format specifier"><p>"ss"</p></td><td data-th="Description"><p>The second, from 00 through 59.</p><p>More information: <a href="#ssSpecifier">The "ss" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:09 -&gt; 09</p></td></tr><tr><td data-th="Format specifier"><p>"t"</p></td><td data-th="Description"><p>The first character of the AM/PM designator.</p><p>More information: <a href="#tSpecifier">The "t" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; P (en-US)</p><p>2009-06-15T13:45:30 -&gt; 午 (ja-JP)</p><p>2009-06-15T13:45:30 -&gt;  (fr-FR)</p></td></tr><tr><td data-th="Format specifier"><p>"tt"</p></td><td data-th="Description"><p>The AM/PM designator.</p><p>More information: <a href="#ttSpecifier">The "tt" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; PM (en-US)</p><p>2009-06-15T13:45:30 -&gt; 午後 (ja-JP)</p><p>2009-06-15T13:45:30 -&gt;  (fr-FR)</p></td></tr><tr><td data-th="Format specifier"><p>"y"</p></td><td data-th="Description"><p>The year, from 0 to 99.</p><p>More information: <a href="#ySpecifier">The "y" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>0001-01-01T00:00:00 -&gt; 1</p><p>0900-01-01T00:00:00 -&gt; 0</p><p>1900-01-01T00:00:00 -&gt; 0</p><p>2009-06-15T13:45:30 -&gt; 9</p><p>2019-06-15T13:45:30 -&gt; 19</p></td></tr><tr><td data-th="Format specifier"><p>"yy"</p></td><td data-th="Description"><p>The year, from 00 to 99.</p><p>More information: <a href="#yySpecifier">The "yy" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>0001-01-01T00:00:00 -&gt; 01</p><p>0900-01-01T00:00:00 -&gt; 00</p><p>1900-01-01T00:00:00 -&gt; 00</p><p>2019-06-15T13:45:30 -&gt; 19</p></td></tr><tr><td data-th="Format specifier"><p>"yyy"</p></td><td data-th="Description"><p>The year, with a minimum of three digits.</p><p>More information: <a href="#yyySpecifier">The "yyy" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>0001-01-01T00:00:00 -&gt; 001</p><p>0900-01-01T00:00:00 -&gt; 900</p><p>1900-01-01T00:00:00 -&gt; 1900</p><p>2009-06-15T13:45:30 -&gt; 2009</p></td></tr><tr><td data-th="Format specifier"><p>"yyyy"</p></td><td data-th="Description"><p>The year as a four-digit number.</p><p>More information: <a href="#yyyySpecifier">The "yyyy" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>0001-01-01T00:00:00 -&gt; 0001</p><p>0900-01-01T00:00:00 -&gt; 0900</p><p>1900-01-01T00:00:00 -&gt; 1900</p><p>2009-06-15T13:45:30 -&gt; 2009</p></td></tr><tr><td data-th="Format specifier"><p>"yyyyy"</p></td><td data-th="Description"><p>The year as a five-digit number.</p><p>More information: <a href="#yyyyySpecifier">The "yyyyy" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>0001-01-01T00:00:00 -&gt; 00001</p><p>2009-06-15T13:45:30 -&gt; 02009</p></td></tr><tr><td data-th="Format specifier"><p>"z"</p></td><td data-th="Description"><p>Hours offset from UTC, with no leading zeros.</p><p>More information: <a href="#zSpecifier">The "z" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30-07:00 -&gt; -7</p></td></tr><tr><td data-th="Format specifier"><p>"zz"</p></td><td data-th="Description"><p>Hours offset from UTC, with a leading zero for a single-digit value.</p><p>More information: <a href="#zzSpecifier">The "zz" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30-07:00 -&gt; -07</p></td></tr><tr><td data-th="Format specifier"><p>"zzz"</p></td><td data-th="Description"><p>Hours and minutes offset from UTC.</p><p>More information: <a href="#zzzSpecifier">The "zzz" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30-07:00 -&gt; -07:00</p></td></tr><tr><td data-th="Format specifier"><p>":"</p></td><td data-th="Description"><p>The time separator.</p><p>More information: <a href="#timeSeparator">The ":" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; : (en-US)</p><p>2009-06-15T13:45:30 -&gt; . (it-IT)</p><p>2009-06-15T13:45:30 -&gt; : (ja-JP)</p></td></tr><tr><td data-th="Format specifier"><p>"/"</p></td><td data-th="Description"><p>The date separator.</p><p>More Information: <a href="#dateSeparator">The "/" Custom Format Specifier</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 -&gt; / (en-US)</p><p>2009-06-15T13:45:30 -&gt; - (ar-DZ)</p><p>2009-06-15T13:45:30 -&gt; . (tr-TR)</p></td></tr><tr><td data-th="Format specifier"><p>"<em>string</em>"</p><p>'<em>string</em>'</p></td><td data-th="Description"><p>Literal string delimiter. </p><p>More information: <a href="#Literals">Character literals</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 ("arr:" h:m t) -&gt; arr: 1:45 P</p><p>2009-06-15T13:45:30 ('arr:' h:m t) -&gt; arr: 1:45 P</p></td></tr><tr><td data-th="Format specifier"><p>%</p></td><td data-th="Description"><p>Defines the following character as a custom format specifier.</p><p>More information:<a href="#UsingSingleSpecifiers">Using Single Custom Format Specifiers</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 (%h) -&gt; 1</p></td></tr><tr><td data-th="Format specifier"><p>\</p></td><td data-th="Description"><p>The escape character.</p><p>More information: <a href="#Literals">Character literals</a> and <a href="#escape">Using the Escape Character</a>.</p></td><td data-th="Examples"><p>2009-06-15T13:45:30 (h \h) -&gt; 1 h</p></td></tr><tr><td data-th="Format specifier"><p>Any other character</p></td><td data-th="Description"><p>The character is copied to the result string unchanged.</p><p>More information: <a href="#Literals">Character literals</a>.</p></td><td data-th="Examples"><p>2009-06-15T01:45:30 (arr hh:mm t) -&gt; arr 01:45 A</p></td></tr></tbody></table></div>

# [Ruby](#ruby)
([source](http://apidock.com/ruby/DateTime/strftime#307-Formatting-options))

%a - The abbreviated weekday name (“Sun”)

%A - The full weekday name (“Sunday”)

%b - The abbreviated month name (“Jan”)

%B - The full month name (“January”)

%c - The preferred local date and time representation

%d - Day of the month (01..31)

%H - Hour of the day, 24-hour clock (00..23)

%I - Hour of the day, 12-hour clock (01..12)

%j - Day of the year (001..366)

%m - Month of the year (01..12)

%M - Minute of the hour (00..59)

%p - Meridian indicator (“AM” or “PM”)

%S - Second of the minute (00..60)

%U - Week number of the current year, starting with the first Sunday as the first day of the first week (00..53)

%W - Week number of the current year, starting with the first Monday as the first day of the first week (00..53)

%w - Day of the week (Sunday is 0, 0..6)

%x - Preferred representation for the date alone, no time

%X - Preferred representation for the time alone, no date

%y - Year without a century (00..99)

%Y - Year with century

%Z - Time zone name %% - Literal “%’’ character t = Time.now t.strftime(“Printed on %m/%d/%Y”) #=> “Printed on 04/09/2003” t.strftime(“at %I:%M%p”) #=> “at 08:56AM”

# [JS](#js)

## [Moment](#moment) 
([source](http://momentjs.com/docs/#/parsing/string-format/))

<h4 id="year-month-and-day-tokens">Year, month, and day tokens</h4>
<table>
<thead>
<tr>
<th>Input</th>
<th>Example</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>YYYY</code></td>
<td><code>2014</code></td>
<td>4 or 2 digit year</td>
</tr>
<tr>
<td><code>YY</code></td>
<td><code>14</code></td>
<td>2 digit year</td>
</tr>
<tr>
<td><code>Y</code></td>
<td><code>-25</code></td>
<td>Year with any number of digits and sign</td>
</tr>
<tr>
<td><code>Q</code></td>
<td><code>1..4</code></td>
<td>Quarter of year. Sets month to first month in quarter.</td>
</tr>
<tr>
<td><code>M MM</code></td>
<td><code>1..12</code></td>
<td>Month number</td>
</tr>
<tr>
<td><code>MMM MMMM</code></td>
<td><code>Jan..December</code></td>
<td>Month name in locale set by <code>moment.locale()</code></td>
</tr>
<tr>
<td><code>D DD</code></td>
<td><code>1..31</code></td>
<td>Day of month</td>
</tr>
<tr>
<td><code>Do</code></td>
<td><code>1st..31st</code></td>
<td>Day of month with ordinal</td>
</tr>
<tr>
<td><code>DDD DDDD</code></td>
<td><code>1..365</code></td>
<td>Day of year</td>
</tr>
<tr>
<td><code>X</code></td>
<td><code>1410715640.579</code></td>
<td>Unix timestamp</td>
</tr>
<tr>
<td><code>x</code></td>
<td><code>1410715640579</code></td>
<td>Unix ms timestamp</td>
</tr>
</tbody>
</table>
<p><code>YYYY</code> from version <strong>2.10.5</strong> supports 2 digit years, and converts them to a year
near 2000 (same as <code>YY</code>).</p>
<p><code>Y</code> was added in <strong>2.11.1</strong>. It will match any number, signed or unsigned. It is useful for years that are not 4 digits or are before the common era. It can be used for any year.</p>

<h4 id="week-year-week-and-weekday-tokens">Week year, week, and weekday tokens</h4>
<p>For these, the lowercase tokens use the locale aware week start days, and the uppercase tokens use the <a href="http://en.wikipedia.org/wiki/ISO_week_date">ISO week date</a> start days.</p>
<table>
<thead>
<tr>
<th>Input</th>
<th>Example</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>gggg</code></td>
<td><code>2014</code></td>
<td>Locale 4 digit week year</td>
</tr>
<tr>
<td><code>gg</code></td>
<td><code>14</code></td>
<td>Locale 2 digit week year</td>
</tr>
<tr>
<td><code>w ww</code></td>
<td><code>1..53</code></td>
<td>Locale week of year</td>
</tr>
<tr>
<td><code>e</code></td>
<td><code>0..6</code></td>
<td>Locale day of week</td>
</tr>
<tr>
<td><code>ddd dddd</code></td>
<td><code>Mon...Sunday</code></td>
<td>Day name in locale set by <code>moment.locale()</code></td>
</tr>
<tr>
<td><code>GGGG</code></td>
<td><code>2014</code></td>
<td>ISO 4 digit week year</td>
</tr>
<tr>
<td><code>GG</code></td>
<td><code>14</code></td>
<td>ISO 2 digit week year</td>
</tr>
<tr>
<td><code>W WW</code></td>
<td><code>1..53</code></td>
<td>ISO week of year</td>
</tr>
<tr>
<td><code>E</code></td>
<td><code>1..7</code></td>
<td>ISO day of week</td>
</tr>
</tbody>
</table>
<h4 id="hour-minute-second-millisecond-and-offset-tokens">Hour, minute, second, millisecond, and offset tokens</h4>
<table>
<thead>
<tr>
<th>Input</th>
<th>Example</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>H HH</code></td>
<td><code>0..23</code></td>
<td>24 hour time</td>
</tr>
<tr>
<td><code>h hh</code></td>
<td><code>1..12</code></td>
<td>12 hour time used with <code>a A</code>.</td>
</tr>
<tr>
<td><code>a A</code></td>
<td><code>am pm</code></td>
<td>Post or ante meridiem (Note the one character <code>a p</code> are also considered valid)</td>
</tr>
<tr>
<td><code>m mm</code></td>
<td><code>0..59</code></td>
<td>Minutes</td>
</tr>
<tr>
<td><code>s ss</code></td>
<td><code>0..59</code></td>
<td>Seconds</td>
</tr>
<tr>
<td><code>S SS SSS</code></td>
<td><code>0..999</code></td>
<td>Fractional seconds</td>
</tr>
<tr>
<td><code>Z ZZ</code></td>
<td><code>+12:00</code></td>
<td>Offset from UTC as <code>+-HH:mm</code>, <code>+-HHmm</code>, or <code>Z</code></td>
</tr>
</tbody>
</table>
