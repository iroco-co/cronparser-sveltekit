<script lang="ts">
  import CronParser from "cron-parser";

  let cronExpression = '*/2 * * * *'
  let interval = CronParser.parseExpression(cronExpression);
</script>

<h1>Welcome to SvelteKit + cron-parser + luxon</h1>
<div>
  next interval for {cronExpression}: {interval.next()}
</div>
