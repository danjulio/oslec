## My modifications to spandsp/OSLEC

This repository contains a fork of Steve Underwood's fantastic spandsp telephony library with David Rowe's incredible OSLEC line echo cancellation code.  I am using this with my weeBell project and made some changes to support that.

The original README.txt file is unchanged.

### Changes
1. spandsp/super\_tone\_tx - Added new API call ```super_tone_tx_make_step_4()``` and increased internal support for up to 4 channels of DDS generated tones.  This allowed me to generate the 4 simultaneous tones used in the North American off-hook sound.