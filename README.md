# Skippy-1Timer-Never-Get-Busted-gen-lang-client-0592095889-
Skippy 1Timer Never Get Busted (gen-lang-client-0592095889)

Matthew Shannon Amos

Skippy-1Timer-Never-Get-Busted-gen-lang-client-0592095889-

       <iframe src="https://www.facebook.com/plugins/video.php?height=314&href=https%3A%2F%2Fwww.facebook.com%2Fmatthew.shannon.amos%2Fvideos%2F1877886542814303%2F&show_text=false&width=560&t=0" width="560" height="314" style="border:none;overflow:hidden" scrolling="no" frameborder="0" allowfullscreen="true" allow="autoplay; clipboard-write; encrypted-media; picture-in-picture; web-share" allowFullScreen="true"></iframe>https://www.facebook.com/matthew.shannon.amos/videos/25554090587541537/
const fs = require('fs');
const puppeteer = require('puppeteer'); // v23.0.0 or later

(async () => {
    const browser = await puppeteer.launch();
    const page = await browser.newPage();
    const timeout = 5000;
    page.setDefaultTimeout(timeout);

    const lhApi = await import('lighthouse'); // v10.0.0 or later
    const flags = {
        screenEmulation: {
            disabled: true
        }
    }
    const config = lhApi.desktopConfig;
    const lhFlow = await lhApi.startFlow(page, {name: 'https://github.com/rainwizzardlivestream-source/Skippy-1Timer-Never-Get-Busted-gen-lang-client-0592095889-/tree/main', config, flags});
    {
        const targetPage = page;
        await targetPage.setViewport({
            width: 1034,
            height: 830
        })
    }
    await lhFlow.startNavigation();
    {
        const targetPage = page;
        await targetPage.goto('https://docs.google.com/videos/d/1JZOZgtB5fcl68caqhCddi2D0QcZBtqEj9rvz_2NlTlo/play');
    }
    await lhFlow.endNavigation();
    await lhFlow.startTimespan();
    {
        const targetPage = page;
        await puppeteer.Locator.race([
            targetPage.locator('div.appsElementsMediaPlaybackRichControlsPlaybackControlsContainer span:nth-of-type(1) > button > div'),
            targetPage.locator('::-p-xpath(/html/body/div[3]/div[3]/div/div[4]/section/div[3]/div[3]/div[1]/div[2]/span/span[1]/button/div)'),
            targetPage.locator(':scope >>> div.appsElementsMediaPlaybackRichControlsPlaybackControlsContainer span:nth-of-type(1) > button > div')
        ])
            .setTimeout(timeout)
            .click({
              offset: {
                x: 23,
                y: 20,
              },
            });
    }
    {
        const targetPage = page;
        await puppeteer.Locator.race([
            targetPage.locator('div.appsElementsMediaPlaybackRichControlsPlayPauseButtonContainer button > div'),
            targetPage.locator('::-p-xpath(/html/body/div[3]/div[3]/div/div[4]/section/div[3]/div[3]/div[1]/div[1]/span/button/div)'),
            targetPage.locator(':scope >>> div.appsElementsMediaPlaybackRichControlsPlayPauseButtonContainer button > div')
        ])
            .setTimeout(timeout)
            .click({
              offset: {
                x: 12,
                y: 15,
              },
            });
    }
    {
        const targetPage = page;
        await puppeteer.Locator.race([
            targetPage.locator('div.appsElementsMediaPlaybackRichControlsSeekingSliderContainer > div'),
            targetPage.locator('::-p-xpath(/html/body/div[3]/div[3]/div/div[4]/section/div[3]/div[2]/div)'),
            targetPage.locator(':scope >>> div.appsElementsMediaPlaybackRichControlsSeekingSliderContainer > div')
        ])
            .setTimeout(timeout)
            .click({
              delay: 1212.699999999255,
              offset: {
                x: 181,
                y: 4,
              },
            });
    }
    {
        const targetPage = page;
        await puppeteer.Locator.race([
            targetPage.locator('div.appsElementsMediaPlaybackRichControlsSeekingSliderContainer > div'),
            targetPage.locator('::-p-xpath(/html/body/div[3]/div[3]/div/div[4]/section/div[3]/div[2]/div)'),
            targetPage.locator(':scope >>> div.appsElementsMediaPlaybackRichControlsSeekingSliderContainer > div')
        ])
            .setTimeout(timeout)
            .click({
              delay: 1304.5,
              offset: {
                x: 351,
                y: 28,
              },
            });
    }
    {
        const targetPage = page;
        await puppeteer.Locator.race([
            targetPage.locator('div.appsElementsMediaPlaybackRichControlsPlayPauseButtonContainer button > div'),
            targetPage.locator('::-p-xpath(/html/body/div[3]/div[3]/div/div[4]/section/div[3]/div[3]/div[1]/div[1]/span/button/div)'),
            targetPage.locator(':scope >>> div.appsElementsMediaPlaybackRichControlsPlayPauseButtonContainer button > div')
        ])
            .setTimeout(timeout)
            .click({
              offset: {
                x: 23,
                y: 24,
              },
            });
    }
    {
        const targetPage = page;
        await puppeteer.Locator.race([
            targetPage.locator('div.appsElementsMediaPlaybackRichControlsPlayPauseButtonContainer button > div'),
            targetPage.locator('::-p-xpath(/html/body/div[3]/div[3]/div/div[4]/section/div[3]/div[3]/div[1]/div[1]/span/button/div)'),
            targetPage.locator(':scope >>> div.appsElementsMediaPlaybackRichControlsPlayPauseButtonContainer button > div')
        ])
            .setTimeout(timeout)
            .click({
              offset: {
                x: 39,
                y: 30,
              },
            });
    }
    await lhFlow.endTimespan();
    const lhFlowReport = await lhFlow.generateReport();
    fs.writeFileSync(__dirname + '/flow.report.html', lhFlowReport)

    await browser.close();

})().catch(err => {
    console.error(err);
    process.exit(1);
});
