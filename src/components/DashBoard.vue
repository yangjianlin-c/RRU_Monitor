<script>
import SerialPort from 'serialport';
SerialPort.list().then((ports) => {
  console.log(ports);
}).catch((error) => {
  console.error(error);
});

</script>
<template>
    <div>dsfad</div>
</template>