---
layout: post
title: "The $50,000 Stick: What Pool Cues Teach Us About Economics"
date: 2026-10-11
description: "Exploring the extreme price variance of billiards equipment, the law of diminishing returns, and the Veblen goods of the pool hall."
tags: [economics, billiards, sports-tech]
categories: [economics-of-pool]
chart:
  plotly: true
---

As a pool player and a financial economist, I have always found the economics of pool fascinating. So, I am starting this series to look at the economics of pool, beginning with a piece of equipment that defies almost every logical rule of the modern sports market. 

Imagine the finals of a World 9-Ball Championship. The lights are hot, the crowd is silent, and hundreds of thousands of dollars ($250,000 to the winner!) are on the line. When a player steps up to the table to face a table-length tough shot, you would expect them to be holding the absolute pinnacle of modern sports engineering, likely a lab tested, carbon fiber cue provided by a massive corporate sponsor. 

But for years, if you watched World Champions like Taiwan's Ko Pin-yi or his brothers, you would see something completely different. 

Before their recent sponsorship deals, the Ko brothers were famously not sponsored by cue makers, stepping up to the biggest shots of their lives holding traditional Southwest cues. They were leaving lucrative cue sponsorship money on the table, bypassing mathematically "perfect" low deflection technology, to play with a traditional wooden custom cue. 

In almost any other sport, this is unthinkable. A PGA Tour golfer does not turn down a TaylorMade sponsorship to play with a wooden driver they bought themselves. 

But billiards is not like other sports. The Ko brothers played with Southwest cues for a very specific reason: the subjective, tactile feedback known in the pool world simply as "the hit." 

This introduces the central paradox of the billiards market. It is a space where the line between a highly engineered athletic tool and an artisan masterpiece is entirely blurred. As a result, the price range for pool cues is wider than any other sports equipment I can think of. A functional, mass-produced Chinese cue will cost you \\$100 to \\$200. A reputable professional brand with state-of-the-art technology maxes out around \\$1,000. But if you want a custom Southwest, or a masterpiece from a maker like Zen or Black Boar? You are looking at waitlists spanning a decade and price tags ranging from \\$10,000 to over \\$50,000. 

## Economic Principle 1: The Staircase of Diminishing Returns

In economics, the Law of Diminishing Marginal Returns states that at a certain point, adding more investment yields progressively smaller increases in actual output. In the billiards market, this law is practically carved into the wood. 

If we plot the pure *performance* of a pool cue against its price, the curve is not a smooth line—it is a staircase of distinct technological jumps that eventually hits a hard ceiling.

**The Super-Cheap Baseline (\\$20–\\$100): The House Cue**
At the absolute bottom, you have the warped bar cue or ultra-cheap import. The tips are rock hard, the wood is rarely straight, and deflection is massive. Performance here is arguably negative; the tool actively hurts your game. 

**Decent Quality (\\$100–\\$300): The Initial Jump**
Moving from a house cue to a decent entry level cue (like a Players or McDermott Lucky or Viking Vahalla) provides the highest return on investment in the sport. You are paying for a straight maple shaft, a usable leather tip, and a solid joint. At this stage, every dollar spent directly translates into consistency.

**The Wood Low-Deflection Era (\\$300–\\$450): Engineering the Shot**
This is the first major technological leap. Shafts in this range (like the Predator 314 series, sitting around \\$360, or Cuetec Avid cues, starting at \\$289) introduce engineered, laminated wood or other materials. The front end of the shaft is hollowed out to reduce mass, physically reducing cue ball squirt deflection when applying side spin. You are paying for a measurable, physical advantage. This is also where the lower priced carbon fiber shafts live, like JFlowers entry level cues. 

**The Carbon Fiber Shaft (\\$450–\\$600): Maximum Utility**
Here is the most fascinating quirk of the billiards market: the absolute pinnacle of functional cue technology has a hard price ceiling. Today, aerospace grade carbon fiber composite shafts are universally recognized as the lowest-deflection equipment in the world. But whether you buy a Cuetec Cynergy (~\\$449), a Predator REVO (~\\$549), or a Mezz Ignite (~\\$599), the market for performance tops out at \\$600. Because the shaft contains most of the technology of the pool cue, that \\$600 represents the maximum price of objective utility.

**High-End Production (\\$700–\\$2,500): The Shift to Aesthetics**
So what happens when a player buys a high end production cue that retails for \\$1,200? If the carbon fiber shaft doing all the work only costs \\$550, what is the other $650 paying for? We have hit the point of diminishing marginal returns. That extra capital is buying a premium butt, you get. (potentially) better balance, exotic wood handles, and custom inlays. The performance gains are practically zero outside of weight and balance, but the aesthetic and craftsmanship value begins to rise.

**The Custom Artisan Realm (\\$10,000–\\$50,000+): The Flatline**
By the time we reach the realm of the \\$10,000 Southwest or the \\$50,000 Zen cue, the objective performance curve has entirely flatlined. A \\$50,000 cue does not pocket balls 50 times better than a \\$1,000 cue. In fact, because these luxury cues often utilize traditional solid wood shafts rather than carbon fiber, many modern professionals would mathematically shoot *worse* with a \\$30,000 masterpiece. 

At this tier, you are no longer paying for utility. The economic value has shifted entirely to a Veblen good.

## The Exception: Subjective Utility and "The Hit"

Just when you think a \\$10,000 cue is purely about conspicuous consumption, we must return to the Ko brothers. 

In Asian pool culture, particularly in Taiwan, custom cues are often considered superior for high-level play. While Western players rely heavily on the objective engineering of carbon fiber, Taiwanese coaches often argue that mass produced shafts lack "stopping power" or the solid feedback required for absolute elite cue ball control. 

This introduces the economic concept of **Subjective Utility**. While a carbon fiber Predator can prove its low deflection with physics and data, the "hit" of an ebony Southwest provides a tactile feedback that elite players genuinely believe gives them a competitive edge. When a professional player feels they can control the cue ball 1% better because of how the wood resonates in their grip, that \\$10,000 price tag isn't conspicuous consumption anymore—it is a functional investment in their livelihood.

---

### Visualize the Market: Performance vs. Price
```plotly
{
  "data": [
    {
      "x": [50, 200, 400, 550, 1200, 3500, 10000, 50000],
      "y": [20, 75, 88, 98, 100, 100, 100, 100],
      "mode": "lines+markers",
      "name": "Performance Utility (%)",
      "line": {
        "shape": "spline",
        "width": 4,
        "color": "#1f77b4"
      },
      "marker": {
        "size": 8
      }
    }
  ],
  "layout": {
    "title": {
      "text": "The Law of Diminishing Returns in Pool Cues"
    },
    "xaxis": {
      "type": "log",
      "title": {
        "text": "Price (USD) - Logarithmic Scale"
      },
      "tickvals": [50, 200, 550, 1200, 10000, 50000],
      "ticktext": ["\\$50", "\\$200", "\\$550 (Carbon Fiber)", "\\$1.2K", "\\$10K", "\\$50K+"]
    },
    "yaxis": {
      "title": {
        "text": "Performance (%)"
      },
      "range": [0, 110]
    },
    "annotations": [
      {
        "x": 2.74036,
        "y": 98,
        "xref": "x",
        "yref": "y",
        "text": "The Carbon Fiber Ceiling",
        "showarrow": true,
        "arrowhead": 2,
        "ax": -40,
        "ay": -40
      },
      {
        "x": 4,
        "y": 100,
        "xref": "x",
        "yref": "y",
        "text": "Value shifts entirely to Art/Prestige",
        "showarrow": true,
        "arrowhead": 2,
        "ax": 0,
        "ay": 40
      }
    ],
    "hovermode": "closest"
  }
}
```

