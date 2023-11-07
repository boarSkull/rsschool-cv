# CV#1.Markdown and git

1. Full Name:
   Kozlov Stanislav

2. Contacts:

   - Gmail: kazemirova.l@gmail.com
   - GitHub: [boarSkull](https://github.com/boarSkull)
   - [Telegram](https://t.me/stas12412)

3. About myself:
   I am a university graduate. Its been a long and hard path for me to get through.
   Unfortunately, the lack of any motivation has led to a meager amount of knowledge, which was barely enough for the implementation of the graduation project. After graduation I tried to get a job, but I can only successfully pass HR specialist and a stumbling block in the form of a technical interview.
   Realizing the complexity of the current situation, I decided to strengthen my knowledge so that it would be sufficient for employment

===

4. Skills:
   - _C#_
   - _EF Core_
   - _HTML&CSS_
   - _a bit of ASP.NET CORE_
   - _SQL_
   - _JavaScript_
   - _React basics_
   - _Node.js basics_

===

5. Code example:
   **_Sum of Intervals 4kyu_**
   function sumIntervals(intervals) {
   let result = [];
   intervals.sort((a, b) => a[0] - b[0]);
   console.log(intervals);
   let tmp = [];
   let currentInterval = intervals[0];
   for (let i = 1; i < intervals.length; i++) {
   if (intervals[i][0] <= currentInterval[1]) {
   currentInterval[1] = Math.max(currentInterval[1], intervals[i][1]);
   } else {
   tmp.push([...currentInterval]);
   currentInterval = intervals[i];
   }
   }
   tmp.push([...currentInterval]);
   console.log(tmp);
   if (tmp.length === 1) {
   return tmp[0][1] - tmp[0][0];
   } else {
   let result = 0;
   for (const arr of tmp) {
   result += arr[1] - arr[0];
   }
   return result;
   }
   }

===

7. Education:
   - Finished basic .Net Training at EPAM during summer practice at university.
   - Learned js at [learn javascript ru](https://learn.javascript.ru/)

===

8. Foreign language:
   In the 10th(2017) grade I certificated B2 level in the international house at Minsk.
   But its been 5 years so probably B1.
