---
share: true
---

# ecto and elixir
> i asked it to write an ecto query for miatapartpicker, i feel like i gave it sufficient context and asked a relatively clear question and it should have been a pretty straightforward answer, but it dicked around making the most complicated query i've ever seen for like 4 tries before giving up trying something else and then ultimately failing
- [Original](https://chat.openai.com/share/305dc3d9-dbb3-4d9c-bf3d-c1a0f98a2ebc)

## GPT 3.5
- 0-Prompt w/o changes (original)
- [1-My version of your prompt](https://chat.openai.com/share/69b64a47-766d-4dcc-8f7d-63528d44d313)

## GPT-4
- [2-Prompt w/o changes](https://chat.openai.com/share/bb1f26a9-54c9-41c0-8b51-d0af57f27f7c)
- [3-My version of your prompt](https://chat.openai.com/share/8c2bd714-9345-486c-b9d2-059015621b68)

# Parts Search
> here's one that i thought should have been pretty easy, but it spit out garbage, probably because i used really poor prompts, but i think it shows my general misuse/misunderstanding quite well. I asked it something i already knew the answer too, it gave me the wrong answer, i corrected it, it then gave me a kind of correct answer to my prompt but not really

> https://chat.openai.com/share/6f94f467-e04b-4712-b6cd-dfabeea7cfa5
also, if there's a way i don't have to see it appologize to me every single time it fucks up, that would be amazing
btw the answer it gave me was straight-up just wrong in this case. it's almost, kind of correct, but not really

You're asking too much, dataset is limit to 2021. 

If you had web browsing, it can't really search LCSC, web crawling blows for bots. If it had an API to access it could do a lot better.
- [4-My attempt at searching for stm parts](https://chat.openai.com/share/f766e6d9-1014-48e7-b0e9-8656f0b582d2)

# Jtag
- [Original](https://chat.openai.com/share/6f94f467-e04b-4712-b6cd-dfabeea7cfa5)
- I think this one might be helped by including detail about what you're trying to achieve as part of your prompt
- You might be better off describing your end game first and then outline these steps you want it to do to achieve it
- the addition of the [APE Prompt - Let's work this out step by step](./APE%20Prompt%20-%20Let's%20work%20this%20out%20step%20by%20step.md) would help a lot too I bet