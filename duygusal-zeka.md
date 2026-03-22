---
layout: default
title: Duygusal Zeka ve Öz Farkındalık
permalink: /duygusal-zeka/
---

<div style="text-align:center; margin-top:20px;">
    <h1 style="font-family: 'Playfair Display', serif; color: var(--primary);">Duygusal Zeka ve Öz Farkındalık</h1>
    <a href="/" style="color: #666; text-decoration: underline;">Ana Sayfaya Dön</a>
</div>

<div class="container" style="max-width: 1200px; margin: 40px auto; padding: 0 15px;">
    <div class="gallery" style="display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 20px;">
        
        {% for post in site.posts %}
            {% if post.kategori == 'Duygusal Zeka ve Öz Farkındalık' %}
            <a href="{{ post.url }}" class="pin" style="display: block; border-radius: 16px; overflow: hidden; background: white; box-shadow: 0 5px 20px rgba(0,0,0,0.06); transition: transform 0.3s;">
                <img src="{{ post.image }}" loading="lazy" alt="{{ post.title }}" style="width: 100%; height: 200px; object-fit: cover; display: block;">
                <div class="pin-content" style="padding: 15px;">
                    <div class="pin-title" style="font-weight: 700; font-size: 1.1rem; color: #222; margin-bottom: 8px;">{{ post.title }}</div>
                    <div class="pin-cat" style="font-size: 0.8rem; color: var(--primary); font-weight: 700; text-transform: uppercase;">{{ post.kategori }}</div>
                </div>
            </a>
            {% endif %}
        {% endfor %}
        
    </div>
</div>
