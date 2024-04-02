# Read: Class 01

## Study Guide

1. **HTML**
2. **CSS**
3. **JavaScript**
4. **React**
5. **Python**

- Django and Docker
- back-end development

### Practice here for markdown

***Italics***

**cross out text**

~~cross out text~~

#### Look into

- API's
- Databases
- Server side

> This is a blockquote

**Image Below**

![man u image](manchesterunited.png)

***Code Block***

`def compare_leaves(tree1, tree2)`<br>
    `def traverse_push(root, stack)`<br>
        `if root is None:`<br>
            `return`<br>
        `if root.left is None and root.right is None`<br>
            `stack.append(root.value)`<br>
        `traverse_push(root.left, stack)`<br>
        `traverse_push(root.right, stack)`<br>

    stack1, stack2 = [], []<br>

    traverse_push(tree1, stack1)<br>
    traverse_push(tree2, stack2)<br>

    stack1.sort()<br>
    stack2.sort()<br>

    return stack1 ==<br>
