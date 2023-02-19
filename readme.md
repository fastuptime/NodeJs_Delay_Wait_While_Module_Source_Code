const {
    Delay,
    DelayMs
} = require('wait-while');

(async () => {
    console.time();
    await Delay(5).then(() => console.timeEnd());

    console.time();
    await DelayMs(2000).then(() => console.timeEnd());
})();