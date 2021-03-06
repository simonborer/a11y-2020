---
title: "Step 5: ARIA; Linting; Evangelism"
date: 2020-06-10T08:47:11+01:00
publishdate: 2020-06-10T08:47:11+01:00
featured_image: light.jpg
summary: "This week we'll cover accessible inputs and live updates. We'll also look at linting, and talk about evangelism."
---
<section>
    <h2>Here's what we're going to talk about today:</h2>
    <ol role="directory">
        <li class="fragment"><a href="#evangelism">Evangelism</a></li>
        <li class="fragment"><a href="#aGame">A Game</a></li>
        <li class="fragment"><a href="#deepDive">WAI-ARIA deep dive</a></li>
    </ol>
</section>
<section id="evangelism">
    <h2>Evangelism</h2>
    <p><img src="/images/evangelion.png" alt="" style="display: block;max-height: 35vh;margin: 0 auto"></p>
</section>
<section>
    <p>You know a lot already. It won't be long until you're working with someone who knows less than you. They will probably be your boss.</p>
    <p>When you're in a room full of developers, you'll argue differently.</p>
    <p>You will know how to solve problems. You will know the cutting edge of technology. You will feel the inefficiencies start to weigh on you.</p>
</section>
<section>
    <p>What will you do when you're the only person who knows how to make a website accessible?</p>
    <p>What will you do when you're the only person who cares about responsive design? Or load times? Or security?</p>
    <p>You need to make it so your team understands.</p>
    <p>You need to make it so your boss doesn't need to understand.</p>
</section>
<section>
    <h3>When your team can improve</h3>
    <p>If there are improvements you can make within your team without additional resources, present it as an opportunity to make your lives easier, and/or grow your skillset.</p>
    <p>But remember, any solution that starts with 'If everyone would just...' isn't a solution.</p>
    <p>Peer review, linting, automation. A good team holds one another accountable.</p>
</section>
<section id="aGame">
    <h2>A game :)</h2>
    <ul>
        <li class="fragment">In an even number of groups of 3-5...</li>
        <li class="fragment">...you are paired with another group.</li>
        <li class="fragment">Create a scorecard for your group with 4 columns - month, price, profit, and total profit.</li>
        <li class="fragment">Subdivide the latter 3 columns into subcolumns, each labelled alternately &#39;us&#39; and &#39;them&#39;</li>
    </ul>
    <div><small>i.e.</small></div>
    <table>
        <thead>
            <tr>
                <th colspan="8" style="font-size: 1.5rem;text-decoration: underline;">Scorecard</th>
            </tr>
            <tr>
                <th colspan="2" rowspan="2" style="vertical-align: bottom;">Month #</th>
                <th colspan="2" id="price">Price</th>
                <th colspan="2" id="profit">Profit</th>
                <th colspan="2" id="total">Total Profit</th>
            </tr>
            <tr>
                <th style="font-size: .8rem;" aria-labelledby="price">Us</th>
                <th style="font-size: .8rem;" aria-labelledby="price">Them</th>
                <th style="font-size: .8rem;" aria-labelledby="profit">Us</th>
                <th style="font-size: .8rem;" aria-labelledby="profit">Them</th>
                <th style="font-size: .8rem;" aria-labelledby="total">Us</th>
                <th style="font-size: .8rem;" aria-labelledby="total">Them</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td colspan="2">1</td>
                <td>$XX</td>
                <td>$XX</td>
                <td>$XX</td>
                <td>$XX</td>
                <td>$XXX</td>
                <td>$XXX</td>
            </tr>
            <tr>
                <td colspan="2">2</td>
                <td>$XX</td>
                <td>$XX</td>
                <td>$XX</td>
                <td>$XX</td>
                <td>$XXX</td>
                <td>$XXX</td>
            </tr>
        </tbody>
    </table>
</section>
<section>
    <p>Your group is a business. Each month you set the price on your product. Your expenses are absolutely fixed. Bankruptcy is impossible. Your profits are driven entirely by market competition <strong>only with your paired group</strong>.</p>
    <p>Each month, you must write down 6 figures: what price you chose, what price your competitor chose, what profit you made, what profit they made, what total profit you made, and what total profit they made.</p>
    <p>The goal of the game is to maximize your company's profit.</p>
</section>
<section>
    <h3>Price/Profit</h3>
    <p>
        <table>
            <thead>
                <tr>
                    <th>Your price</th>
                    <th>Their price</th>
                    <th>Your profit</th>
                    <th>Their profit</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>$30</td>
                    <td>$30</td>
                    <td>110</td>
                    <td>110</td>
                </tr>
                <tr>
                    <td>$30</td>
                    <td>$20</td>
                    <td>20</td>
                    <td>180</td>
                </tr>
                <tr>
                    <td>$30</td>
                    <td>$10</td>
                    <td>20</td>
                    <td>150</td>
                </tr>
                <tr>
                    <td>$20</td>
                    <td>$30</td>
                    <td>180</td>
                    <td>20</td>
                </tr>
                <tr>
                    <td>$20</td>
                    <td>$20</td>
                    <td>80</td>
                    <td>80</td>
                </tr>
                <tr>
                    <td>$20</td>
                    <td>$10</td>
                    <td>30</td>
                    <td>150</td>
                </tr>
                <tr>
                    <td>$10</td>
                    <td>$30</td>
                    <td>150</td>
                    <td>20</td>
                </tr>
                <tr>
                    <td>$10</td>
                    <td>$20</td>
                    <td>150</td>
                    <td>30</td>
                </tr>
                <tr>
                    <td>$10</td>
                    <td>$10</td>
                    <td>50</td>
                    <td>50</td>
                </tr>
            </tbody>
        </table>
    </p>
</section>
<section>
    <ol>
        <li class="fragment">Who won?</li>
        <li class="fragment">What was your strategy?</li>
        <li class="fragment">Assumptions did you make?</li>
        <li class="fragment">What would you do differently?</li>
    </ol>
</section>
<section>
    <h2>Evangelism (continued)</h2>
    <h3>When you need resources</h3>
    <ol>
        <li class="fragment">Get team buy-in</li>
        <li class="fragment">Explain the cost of the issue</li>
        <li class="fragment">Explain the cost of 2 options, both of which you are ready and willing to implement</li>
    </ol>
</section>
<section id="deepDive">
    <h3>WAI-ARIA deep dive</h3>
    <p><figure><img src="/images/jaws.jpeg" alt=""><figcaption>Jaws > JAWS</figcaption></figure></p>
</section>
<section>
    <p>As we covered earlier, WAI-ARIA, a.k.a. ARIA, is a specification from the W3C that uses element attributes to supplement existing semantics</p>
    <ol>
        <li>to provide more information about your markup, and</li>
        <li>provide information about content that updates without a page refresh.</li>
    </ol>
    <p>This is especially relevant when you are using a front-end javascript framework (Angular, React, Vue, et al.).</p>
</section>
<section>
    <p>Remember that the spec tells us that we should use native semantics when they are available.</p>
    <p>If it's a button, use a <code>&lt;button&gt;</code>.</p>
</section>
<section>
    <h3>ARIA roles</h3>
    <p>The role attribute provides information about an element's purpose.</p>
    <p>The role attribute identifies the element to the screenreader, but it <em>does not</em> recreate the native functionality. That's on you.</p>
</section>
<!-- <section>
    <h3>role="button"</h3>
    <p>Let's say, for whatever reason, you need to make a button out of something that's not &lt;button&gt;,
        &lt;input type='button' /&gt;,
        &lt;input type='submit' /&gt;,
        &lt;input type='reset' /&gt; or
        &lt;input type='image' /&gt;.</p>
    <p><code>role='button'</code> identifies any element as a button to a screenreader. Use this in conjunction with <code>tabindex='0'</code> - the role itself does not make the element focusable.</p>
    <p>Remember, too, that a native HTML button will fire an onclick event when space or enter are pressed - so you're also responsible for recreating that native functionality.</p>
</section> -->
<section>
    <h3>A list of roles you won't often need (if you're coding semantically, and not supporting anything below IE10)</h3>
    <table>
        <thead>
            <tr>
                <th>role value</th>
                <th>native element</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><code>article</code></td>
                <td><code>&lt;article>&lt;/article></code></td>
            </tr>
            <tr>
                <td><code>banner</code></td>
                <td><code>&lt;header>&lt;/header></code></td>
            </tr>
            <tr>
                <td><code>checkbox</code> (or <code>switch</code> if the values are on/off)</td>
                <td><code>&lt;input type="checkbox" /></code></td>
            </tr>
            <tr>
                <td><code>complementary</code></td>
                <td><code>&lt;aside>&lt;/aside></code></td>
            </tr>
            <tr>
                <td><code>definition</code></td>
                <td><code>&lt;dfn>&lt;/dfn></code></td>
            </tr>
            <tr>
                <td><code>form</code></td>
                <td><code>&lt;form>&lt;form></code></td>
            </tr>
            <tr>
                <td><code>heading</code></td>
                <td><code>&lt;h1>&lt;/h1></code> to <code>&lt;h6>&lt;/h6></code>; can also extend semantics thusly: <code>&lt;div role="heading" aria-level="7"></code></td>
            </tr>
            <tr>
                <td><code>img</code></td>
                <td><code>&lt;img src="" alt="" /></code></td>
            </tr>
        </tbody>
    </table>
</section>
<section>
    <h3>A list of roles you won't often need (cont'd)</h3>
    <table>
        <thead>
            <tr>
                <th>role value</th>
                <th>native element</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><code>link</code></td>
                <td><code>&lt;a href="">&lt;/a></code></td>
            </tr>
            <tr>
                <td><code>listbox</code></td>
                <td><code>&lt;select>&lt;option value="dog">Dog&lt;/option>&lt;/select></code></td>
            </tr>
            <tr>
                <td><code>listitem</code> (with <code>list</code>)</td>
                <td><code>&lt;li>&lt;/li></code></td>
            </tr>
            <tr>
                <td><code>main</code></td>
                <td><code>&lt;main>&lt;main></code></td>
            </tr>
            <tr>
                <td><code>math</code></td>
                <td><code>&lt;math xmlns="http://www.w3.org/1998/Math/MathML">&lt;/math></code></td>
            </tr>
            <tr>
                <td><code>navigation</code></td>
                <td><code>&lt;nav>&lt;nav></code></td>
            </tr>
            <tr>
                <td><code>progressbar</code></td>
                <td><code>&lt;progress max="100" value="70">70%&lt;/progress></code></td>
            </tr>
        </tbody>
    </table>
</section>
<section>
    <h3>A list of roles you won't often need (cont'd again)</h3>
    <table>
        <thead>
            <tr>
                <th>role value</th>
                <th>native element</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><code>radio</code> (with <code>radiogroup</code>)</td>
                <td><code>&lt;input type="radio" name="a-group" value="choice"></code></td>
            </tr>
            <tr>
                <td><code>scrollbar</code></td>
                <td>CSS: <code>overflow: auto;</code></td>
            </tr>
            <tr>
                <td><code>search</code></td>
                <td><code>&lt;input type="search" /></code></td>
            </tr>
            <tr>
                <td><code>slider</code></td>
                <td><code>&lt;input type="range" min="0" max="11" /></code></td>
            </tr>
            <tr>
                <td><code>spinbutton</code></td>
                <td><code>&lt;input type="number" min="10" max="100" /></code></td>
            </tr>
            <tr>
                <td><code>textbox</code></td>
                <td><code>&lt;textarea>&lt;/textarea></code></td>
            </tr>
        </tbody>
    </table>
</section>
<section>
    <h3>A list of roles you probably <em>will</em> need</h3>
    <table>
        <thead>
            <tr>
                <th>role value</th>
                <th>component</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><code>application</code></td>
                <td>When your HTML document behaves completely different from a standard html document; probably don't use this. It turns off all standard keyboard shortcuts in most screenreaders.</td>
            </tr>
            <tr>
                <td><code>contentinfo</code></td>
                <td>Information about the document, i.e. copyright.</td>
            </tr>
            <tr>
                <td><code>dialog</code></td>
                <td>A modal, for example</td>
            </tr>
            <tr>
                <td><code>document</code></td>
                <td>Puts the assistive technology into 'reading' mode (which it is by default).</td>
            </tr>
            <tr>
                <td><code>grid</code></td>
                <td>A <em>navigable</em> table, with <code>row</code>, <code>rowheader</code>, <code>cell</code>, and <code>columnheader</code>.</td>
            </tr>
            <tr>
                <td><code>group</code></td>
                <td>A group of UI elements not in a perceivable page section.</td>
            </tr>
            <tr>
                <td><code>log</code></td>
                <td>A chat, for example</td>
            </tr>
        </tbody>
    </table>
</section>
<section>
    <h3>More roles you probably <em>will</em> need</h3>
    <table>
        <thead>
            <tr>
                <th>role value</th>
                <th>component</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><code>log</code></td>
                <td>A chat, for example</td>
            </tr>
            <tr>
                <td><code>marquee</code></td>
                <td>Like a <code>log</code>, but not vital or linear, i.e. a carousel or stock ticker.</td>
            </tr>
            <tr>
                <td><code>menubar</code></td>
                <td>A menu (not necessarily navigation), with <code>menu</code>, <code>menuitem</code>, and <code>menuitemcheckbox</code>.</td>
            </tr>
            <tr>
                <td><code>note</code></td>
                <td>A parenthetical, or "callout".</td>
            </tr>
            <tr>
                <td><code>presentation</code></td>
                <td>Similar in function to aria-hidden,; this role tells the screenreader that the element is decorative, but support for it on natively focusable elements is <a href="http://john.foliot.ca/aria-hidden/" target="_blank">interesting<span class="show-for-sr"> Opens in a new window</span></a>.</p>
                </td>
            </tr>
            <tr>
                <td><code>region</code></td>
                <td>A landmark, but where no other section/landmark element or role applies.</td>
            </tr>
            <tr>
                <td><code>separator</code></td>
                <td>Just a dividing line, like an <code>&lt;hr></code>, but also makes allowances for an interactive "splitter".</td>
            </tr>
        </tbody>
    </table>
</section>
<section>
    <h3>Even more roles you'll</em> need</h3>
    <table>
        <thead>
            <tr>
                <th>role value</th>
                <th>component</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><code>status</code></td>
                <td>A status update message, i.e. "your changes have been saved".</td>
            </tr>
            <tr>
                <td><code>tablist</code></td>
                <td>A group of tabs, with the roles <code>tab</code> (for the tab triggers), and <code>tabpanel</code> (for the content revealed by the tab triggers).</td>
            </tr>
            <tr>
                <td><code>timer</code></td>
                <td>A time keeping element.</td>
            </tr>
            <tr>
                <td><code>toolbar</code></td>
                <td>Same concept as a <code>menubar</code>, except that... well, from what I understand a menubar has words, and a toolbar has icons, but you'd think that would be a moot point, with the icons' alternative text, so...</td>
            </tr>
            <tr>
                <td><code>tooltip</code></td>
                <td>An element that provides additional information when focussed/hovered.</td>
            </tr>
            <tr>
                <td><code>tree</code></td>
                <td>With <code>treeitem</code>, describes a navigable tree structure, like folders and files.</td>
            </tr>
        </tbody>
    </table>
</section>
<section>
    <table>
        <thead><tr>
            <th>Widget attributes</th>
        </tr></thead>
        <tbody>    
            <tr><td><code>aria-autocomplete="none|inline|list|both"</code> (w/ <code>role="combobox|textbox"</code>)</td></tr>
            <tr><td><code>aria-checked="true|false|mixed"</code> (w/ <code>role="checkbox|switch|(etc.)"</code>)</td></tr>
            <tr><td><code>aria-current="page|step|date|location|time|true|false"</code></td></tr>
            <tr><td><code>aria-disabled="true|false"</code></td></tr>
            <tr><td><code>aria-expanded="true|false"</code></td></tr>
            <tr><td><code>aria-haspopup="true|false|menu|listbox|tree|grid|dialog"</code></td></tr>
            <tr><td><code>aria-hidden="true|false|undefined"</code></td></tr>
            <tr><td><code>aria-invalid="true|false|grammar|spelling"</code></td></tr>
            <tr><td><code>aria-label={string}</code> (only for invisible text)</td></tr>
        </tbody>
    </table>
</section>
<section>
    <table>
        <thead>
            <tr>
                <th>Widget attributes (continued so I can fit this junk onto separate slides)</th>
            </tr>
        </thead>
        <tbody> 
            <tr><td><code>aria-level={integer}</code> (w/ <code>role="grid|heading|listitem|row|tablist"</code>)</td></tr>
            <tr><td><code>aria-multiline="true|false"</code> (w/ <code>role="textbox"</code>)</td></tr>
            <tr><td><code>aria-multiselectable="true|false"</code> (w/ <code>role="grid|listbox|tablist|tree"</code>)</td></tr>
            <tr><td><code>aria-orientation="horizontal|vertical|undefined"</code> (w/ <code>role="scrollbar|select|separator|slider|tablist|toolbar"</code>)</td></tr>
            <tr><td><code>aria-pressed="true|false|mixed"</code> (w/ <code>role="button"</code>)</td></tr>
            <tr><td><code>aria-readonly="true|false"</code> (w/ <code>role=checkbox|combobox|grid|gridcell| listbox|radiogroup|slider|spinbutton|textbox"</code>)</td></tr>
            <tr><td><code>aria-required="true|false"</code> (w/ <code>role="combobox|gridcell|listbox|radiogroup|spinbutton|textbox|tree"</code>)</td></tr>
            <tr><td><code>aria-selected="true|false|undefined"</code> (w/ <code>role="gridcell|option|row|tab"</code>)</td></tr>
        </tbody>
    </table>
</section>
<section>
    <table>
        <thead><tr>
            <th>Widget attributes (continued)</th>
        </tr></thead>
        <tbody> 
            <tr><td><code>aria-sort="ascending|descending|none|other"</code> (w/ <code>role="columnheader|rowheader"</code>)</td></tr>
            <tr><td><code>aria-valuemax={number} aria-valuemin={number} aria-valuenow={number}</code> (w/ <code>role="range|scrollbar|separator|slider|spinbutton"</code>)</td></tr>
            <tr><td><code>aria-valuetext={string}</code> (w/ <code>role="range|separator"</code>)</td></tr>
        </tbody>
    </table>
</section>
<section>
    <table>
        <thead><tr>
            <th>Live region attributes</th>
        </tr></thead>
        <tbody> 
            <tr><td><code>aria-live="polite|assertive|off"</code> paired with...</td></tr>
            <tr><td><code>aria-atomic="true|false"</code></td></tr>
            <tr><td><code>aria-relevant="additions|text|removals|all"</code></td></tr>
            <tr><td><code>aria-busy="true|false"</code></td></tr>
        </tbody>
    </table>
</section>
<section>
    <table>
        <thead><tr>
            <th>Implicit live region attributes</th>
        </tr><tr>
            <td>Several roles have implicit live region values:</td>
        </tr></thead>
        <tbody> 
            <tr><td><code>role="alert"</code> has an implicit <code>aria-live="assertive"</code></td></tr>
            <tr><td><code>role="status"</code> and <code>role="log"</code> have an implicit <code>aria-live="polite"</code></td></tr>
            <tr><td><code>role="timer"</code> and <code>role="marquee"</code> have an implicit <code>aria-live="off"</code></td></tr>
            <tr><td>These can be overridden by explicitly declaring <code>aria-live</code> values.</td></tr>
        </tbody>
    </table>
</section>
<section>
    <table>
        <thead><tr>
            <th>Relationship attributes</th>
        </tr></thead>
        <tbody>
        <tr><td><code>role="application|composite|group|textbox" aria-activedescendant={id}</code></td></tr>
<tr>    <td><code>aria-controls={id}</code></td></tr>
<tr>    <td><code>aria-labelledby={id}</code></td></tr>
    <tr><td><code>aria-describedby={id}</code> similar to <code>aria-labelledby</code>, but verbose instead of concise</td></tr>
    <tr><td><code>aria-flowto={id}</code> gives the user the option to move to an element, overriding the source order</td></tr> 
    </tbody>
</table>
    
</section>
<section>
    <table>
        <thead><tr>
            <th>Relationship attributes (continued)</th>
        </tr></thead>
        <tbody>
    <tr><td><code>aria-owns={id}</code> Defines a parent-child relationship when one isn't semantically apparent. To understand how this is different from <code>aria-controls</code>, imagine a carousel. The arrows on the left and right would have <code>aria-controls</code> attributes. The dots at the bottom that correlate to individual slides would have <code>aria-owns</code> attributes.</td></tr>
    <tr><td><code>role="article|listitem|menuitem|option|radio|tab" aria-setsize={integer} aria-posinset={integer}</code> Only required when not all elements from the set are included in the DOM.</td></tr>
</tbody>
</table>
</section>
<section>
    <h3>Examples</h3>
    <p>Let's look at some places where aria attributes might come in handy.</p>
    <h4>Modals</h4>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="rNxeggZ" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="rNxeggZ">
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>
</section>
<section>
    <h4>Live regions</h4>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="abdNeyp" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="abdNeyp">
  <span>See the Pen <a href="https://codepen.io/simonborer/pen/abdNeyp">
  abdNeyp</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>
</section>
<section>
    <h4>Feed</h4>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="bGEpXYJ" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="bGEpXYJ">
  <span>See the Pen <a href="https://codepen.io/simonborer/pen/bGEpXYJ">
  bGEpXYJ</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>
</section>
<section>
    <h4>Form validation</h4>
    <p class="codepen" data-height="265" data-theme-id="light" data-default-tab="html,result" data-user="simonborer" data-slug-hash="qBbaXMr" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="qBbaXMr">
  <span>See the Pen <a href="https://codepen.io/simonborer/pen/qBbaXMr">
  qBbaXMr</a> by Simon Borer (<a href="https://codepen.io/simonborer">@simonborer</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>
</section>
<!-- <section>
    <h3>Praxis: Listening to your reading</h3>
    <p>Your reading this week is <a href='https://webaim.org/projects/screenreadersurvey7/'>https://webaim.org/projects/screenreadersurvey7/</a></p>
    <p>If you have headphones with you, please read it with either <a href='https://www.nvaccess.org/' target='_blank'>NVDA</a> or <a href='https://help.apple.com/voiceover/info/guide/10.12/' target='_blank'>>VoiceOver</a>. Or choose another!</p>
</section> -->
<section>
    <h2>A challenge</h2>
    <p>Create a set of accessible 'tabs'.</p>
    <p>Requirements:</p>
    <ul>
        <li>Roving tabindex</li>
        <li>Panel content is hidden from _everyone_ unless selected</li>
        <li>All styling is done by selecting aria attributes</li>
        <li>Use the roles tablist, tab, and tabpanel</li>
        <li>Use the attributes aria-selected, aria-controls, and aria-labelledby</li>
    </ul>
</section>
