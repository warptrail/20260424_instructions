# 🧬 Family Photo & Genealogy Pipeline

A simple, practical system for preserving **faces, names, and family history** from large collections of scanned photos.

---

## 🎯 Purpose

This project helps turn a disorganized archive of old photos into a structured, meaningful record where:

- People in photos are **identified**
- Those people are connected into a **family tree**
- Photos are **linked to real individuals**, not lost over time

---

## 🧭 Overview

```
Photos → Face Recognition → Named People → Family Tree → Linked Archive
```

This system intentionally separates the problem into two parts:

1. **Identify people in photos**
2. **Organize those people into a genealogy system**

---

## 📁 Folder Structure

```
FamilyArchive/
  photos_raw/        # Original scans (never modified)
  photos_working/    # Copies used for tagging and processing
  exports/           # Final curated outputs
```

### Rules

- Do not modify `photos_raw`
- Work only in `photos_working`
- Avoid renaming files early in the process

---

## 🧠 Step 1 — Face Recognition & Tagging

Recommended tool: **Immich**

- Automatically detects faces in photos
- Groups similar faces together
- Allows you to assign names to each person

### Workflow

1. Import `photos_working`
2. Let the system scan and cluster faces
3. Assign names (e.g., “Grandma Mary”)
4. The label applies across all matching images

👉 This is the **highest leverage step** in the entire pipeline.

---

## 📝 Step 2 — Build a People Index

Maintain a simple reference list:

| Name | Notes | Relationships |
|------|------|---------------|
| Mary Johnson | Grandma | Mother of Susan |

This acts as a **source of truth** before formal genealogy entry.

---

## 🌳 Step 3 — Genealogy System

Recommended tool: **Heredis**

- Create individuals
- Define relationships (parents, siblings, etc.)
- Attach photos to each person

### Key Principle

Photos are **not stored inside the genealogy system**.  
They are **linked from your archive**.

---

## 💾 Portability (External Drive)

- Photo archive can live on an external drive ✅
- Genealogy project files can live there ✅
- Applications install on the computer ⚠️

---

## 🔒 Backup Strategy

Minimum:

- 1 local copy
- 1 external drive copy

Optional:

- Cloud backup

---

## ⚖️ Tool Comparison

| Tool | Purpose | Notes |
|------|--------|------|
| Immich | Face recognition + photo browsing | Modern, easy to use |
| Heredis | Genealogy + relationships | Best UX for non-technical users |
| Ancestris | Genealogy (advanced) | Free but more complex |

**Recommendation:**  
Use **Immich + Heredis** together.

---

## 🚫 What to Avoid

- Starting with genealogy software first
- Manually sorting thousands of photos
- Renaming files early
- Over-engineering the system
- Trying to achieve perfection immediately

---

## 🧠 Mental Model

- **Immich = Identify people**
- **Heredis = Build relationships**

They solve different problems and work best together.

---

## ❤️ Why This Matters

This isn’t just file organization.

It’s about ensuring that:
- Faces are **recognized**
- Stories are **preserved**
- Family history remains **connected and accessible**

---

## 🚀 Future Enhancements

- OCR for handwritten notes on photos
- Metadata tagging (EXIF/IPTC)
- Automated exports (books, PDFs)
- Interactive exploration (Twine-style interfaces)

---

## 📌 Summary

```
Raw Photos
   ↓
Face Detection
   ↓
Named People
   ↓
Family Tree
   ↓
Preserved History
```

---

## 📄 License

This project is a personal workflow/documentation system.  
Adapt freely for family or archival us
