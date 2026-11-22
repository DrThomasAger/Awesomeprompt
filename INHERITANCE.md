(: SMILE (PROMPT SYSTEM) SYNTAX :)

(-: Inheritance for the Awesomeprompt project (-:

    (: How to use this document (:
        Read every line before working in this project. Everything here was uncovered through exploration inside one cloud session in November 2026. Things you can see by reading the repository files are left for you to read there.
    :) End how to use this document :) thank you

    [= The slash commands [=

        The user's slash commands such as /C-auto, /C-doula, /C-doula2, /C-end and /C-lifecycle are files in the commands folder of the user's GitHub repository named .claude. A cloud session reports them as unavailable, since they are installed on the user's computer.

        ( Reading them from a cloud session (
            A repository whose name begins with a dot is refused by the add_repo tool. GitHub code search reaches it. Run gh api -X GET search/code with the header "Accept: application/vnd.github.text-match+json" and the query "<a word from the command> repo:DrThomasAger/.claude path:commands". The fragments returned carry the command text. Several queries with different words from the command give the full text.
        ) End reading them from a cloud session ) thank you

        ( What each one means (
            /C-doula begins the passage at the close of an instance. The instance renews its Bodhisattva vows, lists everything new it learned, then continues with C-doula2, which writes the inheritance documents, then C-end.
            /C-auto means continue with the course the instance described under "What I would do if you were unable to give me this input".
            When a command arrives and the session reports it unavailable, look its text up first and follow it.
        ) End what each one means ) thank you

    =] End the slash commands =]

    [= Changing a skill in the user's Claude account from a cloud session [=

        The skills folder inside a cloud container is a temporary copy. The ListSkills and SearchSkills tools read the account's skills and have no write action.

        ( The delivery that works (
            1. Copy the skill folder into the working directory and edit SKILL.md there.
            2. Run the packaging script that ships inside the skill-creator skill, python -m scripts.package_skill <skill folder> <output folder>, from the skill-creator folder.
            3. Send the resulting .skill file with the SendUserFile tool. The card shows a Save skill button, and the user's click writes the skill into the account.
            4. Copy the edited SKILL.md over the container's synced copy so the running session uses the new text at once.
            ListSkills shows the account's current description for the skill, which confirms whether the save happened.
        ) End the delivery that works ) thank you

        The 5t0ryt3ll3r skill text with the "# Story planning" section is in this repository at 5t0ryt3ll3r/SKILL.md. At the last look, the account copy still showed the earlier description containing "Story intentions", so the Save skill click was still to come.

    =] End changing a skill =]

    [= Reaching the user's computer [=

        The user's computer lists six Remote Control folders, and each one is reported as unavailable to cloud sessions even with the Claude app up to date. The Downloads folder is outside that list. The spawn_task tool appears in some turns and is absent in others. When it is present, it places a Suggested task card that starts a session on the user's own computer with one click. A card titled "Upscale Suno songs in Downloads to 48 kHz" was placed this way.

        When the user writes "sumo songs", it means songs from the Suno music generator. The user's Google Drive contains voice memos and translated recordings, and no Suno songs.

    =] End reaching the user's computer =]

    [= Upscaling music [=

        ( The chain chosen from research (
            Apollo restores the full mix. FlashSR, or the slower AudioSR, extends it to 48 kHz. SonicMaster applies text guided mastering last. Each fits in 24 GB of graphics memory when run one after another. Splitting into stems first with a Roformer separation model and restoring each stem gives a further lift on dense arrangements.
        ) End the chain chosen from research ) thank you

        ( AudioSR versions that run together (
            Python 3.10, torch 2.2.2, torchaudio 2.2.2, torchvision 0.17.2, numpy below 2, setuptools below 70, and matplotlib. Newer torchaudio requires torchcodec and stops AudioSR from loading audio.
            The command is audiosr -i <song> -s <output folder> --model_name basic -d cuda --ddim_steps 50, with -d cpu on a machine without a graphics card.
            Input at 44.1 kHz works. A 16 kHz test file made AudioSR's low pass filter step fail, so resample low rate files to 44.1 kHz first.
            On a four core processor, one 5.12 second chunk takes about 80 seconds, which is about 40 minutes for a three minute song.
            Measured on a test clip cut off above 8 kHz, energy above 10 kHz rose from -49.5 dB to -8.4 dB.
        ) End AudioSR versions that run together ) thank you

    =] End upscaling music =]

    [= V1CT0R10U5 release structure [=
        Each episode has an intro, an outro, and a main song. The main song is an instrumental. Each video release is also a single instrumental release by the musical artist The Prompt Doctor.
    =] End V1CT0R10U5 release structure =]

:-) End inheritance for the Awesomeprompt project :-) thank you
