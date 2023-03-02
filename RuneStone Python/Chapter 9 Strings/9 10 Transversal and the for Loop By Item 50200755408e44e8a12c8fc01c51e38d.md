# 9.10 Transversal and the for Loop: By Item

### **Transversal loops**

- Often we start at the beginning, select each character in turn, do something to it, and continue until the end. This pattern of processing is called a **traversal**

```python
for aname in ["Joe", "Amy", "Brad", "Angelina", "Zuki", "Thandi", "Paris"]:
    invitation = "Hi " + aname + ".  Please come to my party on Saturday!"
    print(invitation)

''' Output
Hi Joe.  Please come to my party on Saturday!
Hi Amy.  Please come to my party on Saturday!
Hi Brad.  Please come to my party on Saturday!
Hi Angelina.  Please come to my party on Saturday!
Hi Zuki.  Please come to my party on Saturday!
Hi Thandi.  Please come to my party on Saturday!
Hi Paris.  Please come to my party on Saturday!
'''
```