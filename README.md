# assignment2-mudhagoni

## Sai Kumar Mudhagoni

###### Maldives

**Maldives** is well known for its crystalline waters with beautiful shades of blue, **swaying palm trees**, and **sparkling white sand** under the **limitless blue skies**. With good weather throughout most of the year, Maldives makes a great choice for an idyllic beach getaway. It is the ultimate dream of **luxury and tranquility**.

---

# Travelling directions
1. Maryville to Maldives 
    1. Maryville to Kansas (MCI)
    2. Kansas to Chicago (ORD)
    3. Chicago to Delhi (IGI)
    4. Delhi to Hyderabad (RGI)
    5. Hyerabad to Maldives (MD)

- Electronic gadgets
- Sheos
- Clothing
- Food items
- Money

[AboutMe](https://github.com/saikumarm007/assignment2-mudhagoni/blob/main/AboutMe.md)

---

# Food/Drink would like to eat everytime
| Food/Drink | Location | Price |
| :---: | :---: | :---: |
| Biryani | Bawarchi | $12 |
| Ice Cream | Pista house | $15 |
| Maggie | BBQ | $5 |
| Shawarma | Mehfil | $10 |
| Cakes | SwissCastle | $3 |        

---
# Quotations
>*"We simply attempt to be fearful when others are greedy and to be greedy only when others are fearful"* <br/>
>*"Price is what you pay. Value is what you get"* <br/>
> - by **Warren Buffet**

---
# Code Fencing

>In computer science, a suffix automaton is an efficient data structure for representing the substring index of a given string which allows the storage, processing, and retrieval of compressed information about all its substrings. The suffix automaton of a string {\displaystyle S}S is the smallest directed acyclic graph with a dedicated initial vertex and a set of "final" vertices, such that paths from the initial vertex to final vertices represent the suffixes of the string.

[Source link for description](https://en.wikipedia.org/wiki/Suffix_automaton)

```
void sa_extend(char c) {
    int cur = sz++;
    st[cur].len = st[last].len + 1;
    int p = last;
    while (p != -1 && !st[p].next.count(c)) {
        st[p].next[c] = cur;
        p = st[p].link;
    }
    if (p == -1) {
        st[cur].link = 0;
    } else {
        int q = st[p].next[c];
        if (st[p].len + 1 == st[q].len) {
            st[cur].link = q;
        } else {
            int clone = sz++;
            st[clone].len = st[p].len + 1;
            st[clone].next = st[q].next;
            st[clone].link = st[q].link;
            while (p != -1 && st[p].next[c] == q) {
                st[p].next[c] = clone;
                p = st[p].link;
            }
            st[q].link = st[cur].link = clone;
        }
    }
    last = cur;
}

```

[Source link for code](https://cp-algorithms.com/string/suffix-automaton.html)

---

# Hi there 👋
- 👨‍🎓 I'm currently pursuing Master's at Northwest Missouri State University.
- 📚 I'm currently learning Webapps with the help from Dr. Charles Hoot.
- ❓ Any queries please ping me in Teams

---

[Profile link](https://github.com/saikumarm007)