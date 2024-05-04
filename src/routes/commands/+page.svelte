<h3>Commands</h3>
<p>
  This list is irregularly updated and does not list all commands, only core ones. Please consult
  the <a href="https://github.com/mblouka/kaabot">repository</a> for up-to-date information.
</p>
<ul>
  <li>
    Cite verses from the Holy Quran with the <code>/verse</code> command. Provides English, Arabic,
    and Urdu translations automatically.
    <ul>
      <li>
        Analyze the individual Arabic words of each verse by passing the optional <code
          >analyse</code
        > parameter.
      </li>
      <li>
        Verses provided from <a href="https://www.openquran.com/">OpenQuran</a>, an easy-to-use
        Quran search engine.
      </li>
    </ul>
  </li>
  <li>
    Cite hadiths from trusted Muslim scholars with the <code>/hadith</code> command.
    <ul>
      <li>
        Give it a single book name and verse reference (e.g. <code>bukhari:6594</code>) and the bot
        will post the relevant paragraph into chat.
      </li>
    </ul>
  </li>
  <li>
    Retrieve interesting commentary of the Holy Quran with the <code>/5v</code> command. Sources
    commentary from the
    <a href="https://www.booksonislam.org/products/five-volume-commentary">Five Volume Commentary</a
    >
    collection (thus <code>5v</code>).
    <ul>
      <li>
        Give it a single verse (e.g. <code>1:1</code>) and the bot will post the relevant page of
        the verse into chat.
      </li>
    </ul>
  </li>
  <li>
    On-demand retrieval of Salat timings with the <code>/salat</code> command, as well as an opt-in
    notifier/reminder for prayers with configurable location(s).
    <ul>
      <li>
        Uses <a href="https://github.com/osm-search/Nominatim">Nominatim</a> for geolocalization. If
        you are hosting Kaab&#39;ot yourself, you will also have to host your own Nominatim instance.
      </li>
      <li>
        <strong>Experimental feature.</strong> Must be manually enabled by administrators of self-hosted
        bots.
      </li>
    </ul>
  </li>
  <li>
    Fetch Friday Sermons from <a href="https://beta.mta.tv/"
      >Muslim Television Ahmadiyya International</a
    >.
    <ul>
      <li>
        Provides both a permalink on MTA <strong>and</strong> a direct download link to a 1920x1080 (full
        HD) MP4 of the sermon.
      </li>
      <li>Pass <code>list</code> parameter to retrieve the last 10 Friday sermons.</li>
    </ul>
  </li>
  <li>
    Retrieval of the Bai&#39;at (initiation into Islam) form, as well as the Conditions of
    Bai&#39;at, with the <code>/baiat</code> command.
    <ul>
      <li>
        Give it a single index from 1 until 10 and the bot will post the relevant Condition of
        Bai&#39;at. If no index is provided, it will provide an explanation of Bai&#39;at and a link
        to the form.
      </li>
    </ul>
  </li>
  <li>
    Access hundreds of selected writings and books from scholars, caliphs and Hazrat Mirza Ghulam
    Ahmad (a.s.).
    <ul>
      <li>
        Local library can be built from alislam.org with the <code>npm run books</code> command. Automatically
        downloads all PDF files too.
      </li>
      <li>
        Search results can be curated with <code>skip</code> and <code>limit</code> parameters to prevent
        listing of 100+ books all at once in a single message.
      </li>
      <li>
        <code>/library search</code> to search through the library with a keyword (e.g., &#39;jesus&#39;).
      </li>
      <li>
        <code>/library get</code> retrieves a book from its unique identifier. Displays a description,
        author information, and a download link to an English PDF.
      </li>
      <li>
        <code>/library download</code> uploads a PDF of the book directly into the Discord channel.
      </li>
      <li><code>/library author</code> searches for, and displays information about, an author.</li>
      <li><code>/library list-books</code> lists the books from an author.</li>
      <li><code>/library list-authors</code> lists all currently indexed authors.</li>
    </ul>
  </li>
  <li>
    Convert between Gregorian and Hijri dates using <code>/calendar</code>, understands both precise
    (e.g., &quot;March 10, 2024&quot;) <strong>and</strong> imprecise/relative (e.g., &quot;next friday&quot;,
    &quot;2 weeks from now&quot;, etc.) inputs.
  </li>
</ul>
