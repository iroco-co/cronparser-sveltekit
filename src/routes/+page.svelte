<script lang="ts">
  import CronParser from "cron-parser"
  import {DateTime} from "luxon";
  let cronExpression = '*/2 * * * *'
  let interval = CronParser.parseExpression(cronExpression);
</script>

<h1>Welcome to SvelteKit + cron-parser + luxon</h1>
<div>
  Now: {DateTime.now().toJSDate()}
</div>
<div>
  Next interval for {cronExpression}: {interval.next()}
</div>
